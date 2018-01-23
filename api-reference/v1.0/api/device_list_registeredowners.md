# <a name="list-registeredowners"></a><span data-ttu-id="a5e9b-101">Listar registeredOwners</span><span class="sxs-lookup"><span data-stu-id="a5e9b-101">List registeredOwners</span></span>

<span data-ttu-id="a5e9b-102">Recupera uma lista de usuários que são proprietários registrados do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a5e9b-102">Retrieve a list of users that are registered owners of the device.</span></span> <span data-ttu-id="a5e9b-103">Um proprietário registrado é o usuário que se associou ao dispositivo na nuvem ou que registrou o dispositivo pessoal.</span><span class="sxs-lookup"><span data-stu-id="a5e9b-103">A registered owner is the user that cloud joined the device or registered their personal device.</span></span> <span data-ttu-id="a5e9b-104">O proprietário registrado é definido no momento do registro.</span><span class="sxs-lookup"><span data-stu-id="a5e9b-104">The registered owner is set at the time of registration.</span></span> <span data-ttu-id="a5e9b-105">Atualmente, só pode haver um proprietário.</span><span class="sxs-lookup"><span data-stu-id="a5e9b-105">Currently, there can be only one owner.</span></span>

## <a name="permissions"></a><span data-ttu-id="a5e9b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a5e9b-106">Permissions</span></span>
<span data-ttu-id="a5e9b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a5e9b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="a5e9b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a5e9b-109">Permission type</span></span>      | <span data-ttu-id="a5e9b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a5e9b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a5e9b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a5e9b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a5e9b-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a5e9b-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a5e9b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a5e9b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5e9b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a5e9b-114">Not supported.</span></span>    |
|<span data-ttu-id="a5e9b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a5e9b-115">Application</span></span> | <span data-ttu-id="a5e9b-116">Device.ReadWrite.All e User.ReadBasic.All ou Directory.Read.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5e9b-116">Device.ReadWrite.All and User.ReadBasic.All or Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a5e9b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a5e9b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredOwners
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a5e9b-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a5e9b-118">Optional query parameters</span></span>
<span data-ttu-id="a5e9b-119">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/pt-BR/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a5e9b-119">This method supports the [OData Query Parameters](http://developer.microsoft.com/pt-BR/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a5e9b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a5e9b-120">Request headers</span></span>
| <span data-ttu-id="a5e9b-121">Nome</span><span class="sxs-lookup"><span data-stu-id="a5e9b-121">Name</span></span>       | <span data-ttu-id="a5e9b-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="a5e9b-122">Type</span></span> | <span data-ttu-id="a5e9b-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5e9b-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a5e9b-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="a5e9b-124">Authorization</span></span>  | <span data-ttu-id="a5e9b-125">string</span><span class="sxs-lookup"><span data-stu-id="a5e9b-125">string</span></span>  | <span data-ttu-id="a5e9b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a5e9b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a5e9b-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a5e9b-128">Request body</span></span>
<span data-ttu-id="a5e9b-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a5e9b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a5e9b-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5e9b-130">Response</span></span>

<span data-ttu-id="a5e9b-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a5e9b-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a5e9b-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a5e9b-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a5e9b-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a5e9b-133">Request</span></span>
<span data-ttu-id="a5e9b-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a5e9b-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_registeredowners"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices/{id}/registeredOwners
```
##### <a name="response"></a><span data-ttu-id="a5e9b-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5e9b-135">Response</span></span>
<span data-ttu-id="a5e9b-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a5e9b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List registeredOwners",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->