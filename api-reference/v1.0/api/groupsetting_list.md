# <a name="list-group-settings"></a><span data-ttu-id="cf7f7-101">Lista de configurações de grupo</span><span class="sxs-lookup"><span data-stu-id="cf7f7-101">List group settings</span></span>

<span data-ttu-id="cf7f7-102">Recuperar uma lista de objetos de configuração de grupo.</span><span class="sxs-lookup"><span data-stu-id="cf7f7-102">Retrieve a list of group setting objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cf7f7-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cf7f7-103">Prerequisites</span></span>

<span data-ttu-id="cf7f7-104">Um dos seguintes **escopos** é obrigatório para executar esta API: *Directory.Read.All*, *Directory.ReadWrite.All* ou *Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="cf7f7-104">One of the following **scopes** is required to execute this API: *Directory.Read.All* or *Directory.ReadWrite.All* or *Directory.AccessAsUser.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="cf7f7-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cf7f7-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="cf7f7-106">Lista configurações de todo o locatário ou específico.</span><span class="sxs-lookup"><span data-stu-id="cf7f7-106">List tenant-wide or group settings.</span></span>

```http
GET /groupSettings
GET group/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cf7f7-107">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="cf7f7-107">Optional query parameters</span></span>
<span data-ttu-id="cf7f7-108">Este método dá suporte a [Parâmetros de consulta OData](http://graph.microsoft.io/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="cf7f7-108">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

> <span data-ttu-id="cf7f7-109">Observação: $filter não é suportado.</span><span class="sxs-lookup"><span data-stu-id="cf7f7-109">Note: $filter is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cf7f7-110">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cf7f7-110">Request headers</span></span>
| <span data-ttu-id="cf7f7-111">Nome</span><span class="sxs-lookup"><span data-stu-id="cf7f7-111">Name</span></span> | <span data-ttu-id="cf7f7-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf7f7-112">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="cf7f7-113">Autorização</span><span class="sxs-lookup"><span data-stu-id="cf7f7-113">Authorization</span></span>  | <span data-ttu-id="cf7f7-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cf7f7-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cf7f7-116">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cf7f7-116">Request body</span></span>
<span data-ttu-id="cf7f7-117">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cf7f7-117">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf7f7-118">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf7f7-118">Response</span></span>

<span data-ttu-id="cf7f7-119">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [groupSetting](../resources/groupsetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cf7f7-119">If successful, this method returns a `200 OK` response code and collection of [groupSetting](../resources/groupsetting.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cf7f7-120">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cf7f7-120">Example</span></span>

##### <a name="request"></a><span data-ttu-id="cf7f7-121">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cf7f7-121">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_groupsettings"
}-->
```http
GET https://graph.microsoft.com/v1.0/groupSettings
```
##### <a name="response"></a><span data-ttu-id="cf7f7-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf7f7-122">Response</span></span>

<span data-ttu-id="cf7f7-p102">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cf7f7-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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