
���ù���docker image �ֿ��ַ

cat /etc/docker/daemon.json 
{
"registry-mirrors": ["https://registry.docker-cn.com"]
}



0 ��������
  docker search
  docker pull mysql  
  docker info
  docker stats  
1 docker images

2 docker ps -a -l

3 docker build -t pez1420/javavul:test . --rm=true
-tѡ��ָ�����ɾ�����û������ֿ�����tag
--rm=trueָ�������ɾ��������ɾ���м��������ʱ������

4 docker images pez1420/javavul
�鿴�²����ľ���

5 ���о���
	docker run -d -p 8090:8080 5207
		-pָ������80�˿�������8080�˿ڽ��а�
		-d ָ���������к��뵱ǰtty���룬��̨����
		5207�Ǿ����IDǰ4λ��

6 ͣ��ȫ�������е�����
docker stop $(docker ps -q)
docker stop 2882c14cefa9(����ID)

7 ɾ����������
docker rm $(docker ps -aq)

8 ��������
docker inspect ���鿴����������ϸ��Ϣ

docker exec -it 8f1b89183df5 /bin/sh   
  8f1b89183df5Ϊ����ID  /bin/sh��Ҫִ�е�����
	-d :����ģʽ: �ں�̨����
	-i :��ʹû�и���Ҳ����STDIN ��
	-t :����һ��α�ն�
  
�����ļ�Ŀ¼:
cd /mnt/hgfs/


8 ɾ��images��ͨ��image��id��ָ��ɾ��˭
docker rmi <image id>

