# <a name="list-group-settings"></a><span data-ttu-id="497ba-101">Lista de configurações de grupo</span><span class="sxs-lookup"><span data-stu-id="497ba-101">List group settings</span></span>

<span data-ttu-id="497ba-102">Recuperar uma lista de objetos de configuração de grupo.</span><span class="sxs-lookup"><span data-stu-id="497ba-102">Retrieve a list of group setting objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="497ba-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="497ba-103">Permissions</span></span>

<span data-ttu-id="497ba-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="497ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="497ba-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="497ba-106">Permission type</span></span>      | <span data-ttu-id="497ba-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="497ba-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="497ba-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="497ba-108">Delegated (work or school account)</span></span> | <span data-ttu-id="497ba-109">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="497ba-109">One of the following scopes is required to execute this API: Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All</span></span>    | 
|<span data-ttu-id="497ba-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="497ba-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="497ba-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="497ba-111">Not supported.</span></span>    | 
|<span data-ttu-id="497ba-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="497ba-112">Application</span></span> | <span data-ttu-id="497ba-113">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="497ba-113">Directory.Read.All, Directory.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="497ba-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="497ba-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="497ba-115">Lista configurações de todo o locatário ou específico.</span><span class="sxs-lookup"><span data-stu-id="497ba-115">List tenant-wide or group settings.</span></span>

```http
GET /groupSettings
GET group/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="497ba-116">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="497ba-116">Optional query parameters</span></span>
<span data-ttu-id="497ba-117">Este método dá suporte a [Parâmetros de consulta OData](http://graph.microsoft.io/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="497ba-117">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

> <span data-ttu-id="497ba-118">Observação: $filter não é suportado.</span><span class="sxs-lookup"><span data-stu-id="497ba-118">Note: $filter is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="497ba-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="497ba-119">Request headers</span></span>
| <span data-ttu-id="497ba-120">Nome</span><span class="sxs-lookup"><span data-stu-id="497ba-120">Name</span></span> | <span data-ttu-id="497ba-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="497ba-121">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="497ba-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="497ba-122">Authorization</span></span>  | <span data-ttu-id="497ba-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="497ba-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="497ba-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="497ba-125">Request body</span></span>
<span data-ttu-id="497ba-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="497ba-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="497ba-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="497ba-127">Response</span></span>

<span data-ttu-id="497ba-128">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [groupSetting](../resources/groupsetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="497ba-128">If successful, this method returns a `200 OK` response code and collection of [groupSetting](../resources/groupsetting.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="497ba-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="497ba-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="497ba-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="497ba-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_groupsettings"
}-->
```http
GET https://graph.microsoft.com/v1.0/groupSettings
```
##### <a name="response"></a><span data-ttu-id="497ba-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="497ba-131">Response</span></span>

<span data-ttu-id="497ba-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="497ba-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 263

{
  "value": [
    {
      "displayName": "displayName-value",
      "templateId": "templateId-value",
      "values": [
        {
          "name": "name-value",
          "value": "value-value"
        }
      ],
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groupSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->