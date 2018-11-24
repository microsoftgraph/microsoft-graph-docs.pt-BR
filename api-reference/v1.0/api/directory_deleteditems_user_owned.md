# <a name="list-deleted-items-owned-by-a-user"></a><span data-ttu-id="38de2-101">**Listar itens excluídos pertencentes a um usuário**</span><span class="sxs-lookup"><span data-stu-id="38de2-101">**List deleted items owned by a user**</span></span>

<span data-ttu-id="38de2-102">Recupera uma lista de itens excluídos recentemente pertencentes ao usuário especificado.</span><span class="sxs-lookup"><span data-stu-id="38de2-102">Retrieves a list of recently deleted items owned by the specified user.</span></span>  

<span data-ttu-id="38de2-103">Atualmente, a funcionalidade de itens de lista excluída é suportada somente para [Agrupar](../resources/group.md) recursos pertencentes ao usuário.</span><span class="sxs-lookup"><span data-stu-id="38de2-103">Currently, list deleted items functionality is supported only for [group](../resources/group.md) resources owned by the user.</span></span>

<span data-ttu-id="38de2-104">Esta é uma ação de serviço, o que significa que ele não dá suporte a paginação.</span><span class="sxs-lookup"><span data-stu-id="38de2-104">This is a service action, which means it does not support pagination.</span></span>  <span data-ttu-id="38de2-105">A API retorna até 1.000 objetos excluídos pertencentes ao usuário, classificado por ID.</span><span class="sxs-lookup"><span data-stu-id="38de2-105">The API returns up to 1,000 deleted objects owned by the user, sorted by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="38de2-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="38de2-106">Permissions</span></span>

<span data-ttu-id="38de2-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="38de2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

| <span data-ttu-id="38de2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="38de2-109">Permission type</span></span> | <span data-ttu-id="38de2-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="38de2-110">Permissions (from least to most privileged)</span></span> |
| --- | --- |
| <span data-ttu-id="38de2-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="38de2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="38de2-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38de2-112">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="38de2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="38de2-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="38de2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="38de2-114">Not supported.</span></span> |
| <span data-ttu-id="38de2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="38de2-115">Application</span></span> | <span data-ttu-id="38de2-116">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38de2-116">Group.Read.All, Group.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="38de2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="38de2-117">HTTP request</span></span>

``` http
POST /directory/deletedItems/getUserOwnedObjects
```

## <a name="request-headers"></a><span data-ttu-id="38de2-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="38de2-118">Request headers</span></span>

| <span data-ttu-id="38de2-119">Nome</span><span class="sxs-lookup"><span data-stu-id="38de2-119">Name</span></span>          | <span data-ttu-id="38de2-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="38de2-120">Description</span></span>               |
| ------------- | ------------------------- |
| <span data-ttu-id="38de2-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="38de2-121">Authorization</span></span> | <span data-ttu-id="38de2-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="38de2-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="38de2-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="38de2-124">Request body</span></span>

```json
{
  "userId":"{id}",
  "type":"Group"
}
```

<span data-ttu-id="38de2-125">O corpo da solicitação requer os seguintes parâmetros:</span><span class="sxs-lookup"><span data-stu-id="38de2-125">The request body requires the following parameters:</span></span>

| <span data-ttu-id="38de2-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="38de2-126">Parameter</span></span>    | <span data-ttu-id="38de2-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="38de2-127">Type</span></span> |<span data-ttu-id="38de2-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="38de2-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="38de2-129">userId</span><span class="sxs-lookup"><span data-stu-id="38de2-129">userId</span></span>|<span data-ttu-id="38de2-130">String</span><span class="sxs-lookup"><span data-stu-id="38de2-130">String</span></span>|<span data-ttu-id="38de2-131">ID do proprietário.</span><span class="sxs-lookup"><span data-stu-id="38de2-131">ID of the owner.</span></span>|
|<span data-ttu-id="38de2-132">type</span><span class="sxs-lookup"><span data-stu-id="38de2-132">type</span></span>|<span data-ttu-id="38de2-133">String</span><span class="sxs-lookup"><span data-stu-id="38de2-133">String</span></span>|<span data-ttu-id="38de2-134">Tipo de objetos pertencentes para retornar; `Group` atualmente é o único valor com suporte.</span><span class="sxs-lookup"><span data-stu-id="38de2-134">Type of owned objects to return; `Group` is currently the only supported value.</span></span>|


## <a name="response"></a><span data-ttu-id="38de2-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="38de2-135">Response</span></span>

<span data-ttu-id="38de2-136">Solicitações bem-sucedidas retornam `200 OK` códigos de resposta; o objeto de resposta inclui propriedades do [diretório (itens excluídos)](../resources/directory.md) .</span><span class="sxs-lookup"><span data-stu-id="38de2-136">Successful requests return `200 OK` response codes; the response object includes [directory (deleted items)](../resources/directory.md) properties.</span></span>

## <a name="example"></a><span data-ttu-id="38de2-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="38de2-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="38de2-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="38de2-138">Request</span></span>

<span data-ttu-id="38de2-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="38de2-139">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/v1.0/directory/deletedItems/getUserOwnedObjects
Content-type: application/json
```

``` json
{
  "userId":"55ac777c-109e-4022-b58c-470c8fcb6892",
  "type":"group"
}
```

###### <a name="response"></a><span data-ttu-id="38de2-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="38de2-140">Response</span></span>

<span data-ttu-id="38de2-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="38de2-141">Here is an example of the response.</span></span> <span data-ttu-id="38de2-142">Observação: Este objeto de resposta pode estar truncado para fins de concisão.</span><span class="sxs-lookup"><span data-stu-id="38de2-142">Note: This response object may be truncated for brevity.</span></span> <span data-ttu-id="38de2-143">Todas as propriedades com suporte são retornadas de chamadas reais.</span><span class="sxs-lookup"><span data-stu-id="38de2-143">All supported properties are returned from actual calls.</span></span>

``` http
HTTP/1.1 200
Content-type: application/json
Content-length: 1249

{
"value": [
          {
              "@odata.type": "#microsoft.graph.group",
              "id": "bfa7033a-7367-4644-85f5-95aaf385cbd7",
              "deletedDateTime": 2018-04-01T12:39:16Z,
              "classification": null,
              "createdDateTime": "2017-03-22T12:39:16Z",
              "description": null,
              "displayName": "Test",
              "groupTypes": [
                  "Unified"
              ],
              "mail": "Test@contoso.com",
              "mailEnabled": true,
              "mailNickname": "Test",
              "membershipRule": null,
              "membershipRuleProcessingState": null,
              "preferredDataLocation": null,
              "preferredLanguage": null,
              "proxyAddresses": [
                  "SMTP:Test@contoso.com"
              ],
              "renewedDateTime": "2017-09-22T22:30:39Z",
              "securityEnabled": false,
              "theme": null,
              "visibility": "Public"
          } 
        ]
 }
```


