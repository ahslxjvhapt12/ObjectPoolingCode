# ObjectPoolingCode

풀링 될 오브젝트를 생성하는 함수
private void CreatePooledObj()

오브젝트를 꺼내오는 함수
꺼내올 오브젝트의 이름을 넣으면 작동
public GameObject PopObj(string objName)

오브젝트를 다시 비활성하는 함수
오브젝트의 이름을 넣으면 Queue에 들어가며 작동
public void PushObj(string objName, GameObject obj)

풀링 된 오브젝트가 저장될 Queue
public Queue<GameObject> objQueue = new Queue<GameObject>();

풀링 될 오브젝트의 네임
public string name;

풀링 될 오브젝트의 갯수
public int maxCount;

풀링 될 오브젝트
public GameObject obj;
