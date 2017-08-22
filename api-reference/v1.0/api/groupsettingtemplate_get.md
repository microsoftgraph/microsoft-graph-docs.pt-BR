# <a name="get-a-group-setting-template"></a><span data-ttu-id="4ca96-101">Obter um modelo de configuração de grupo</span><span class="sxs-lookup"><span data-stu-id="4ca96-101">Get a group setting template</span></span>

<span data-ttu-id="4ca96-p101">Um modelo de configuração de grupo representa um modelo de configurações pelo qual as configurações podem ser criadas dentro de um locatário. Esta operação permite recuperação das propriedades do objeto [groupSettingTemplate](../resources/groupsettingtemplate.md), inclusive as configurações disponíveis e seus padrões.</span><span class="sxs-lookup"><span data-stu-id="4ca96-p101">A group setting template represents a template of settings from which settings may be created within a tenant. This operation allows retrieval of the properties of the [groupSettingTemplate](../resources/groupsettingtemplate.md) object, including the available settings and their defaults.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4ca96-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4ca96-104">Prerequisites</span></span>

<span data-ttu-id="4ca96-105">Os seguintes **escopos** são necessários para executar esta API: *Directory.Read.All*, *Directory.ReadWrite.All* ou *Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="4ca96-105">The following **scopes** are required to execute this API: *Directory.Read.All* or *Directory.ReadWrite.All* or *Directory.AccessAsUser.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="4ca96-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4ca96-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupSettingTemplates/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4ca96-107">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4ca96-107">Optional query parameters</span></span>
<span data-ttu-id="4ca96-108">Este método dá suporte a [Parâmetros de consulta OData](http://graph.microsoft.io/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4ca96-108">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4ca96-109">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4ca96-109">Request headers</span></span>
| <span data-ttu-id="4ca96-110">Nome</span><span class="sxs-lookup"><span data-stu-id="4ca96-110">Name</span></span> | <span data-ttu-id="4ca96-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ca96-111">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="4ca96-112">Autorização</span><span class="sxs-lookup"><span data-stu-id="4ca96-112">Authorization</span></span> | <span data-ttu-id="4ca96-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4ca96-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4ca96-115">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4ca96-115">Request body</span></span>
<span data-ttu-id="4ca96-116">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4ca96-116">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ca96-117">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ca96-117">Response</span></span>

<span data-ttu-id="4ca96-118">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [groupSettingTemplate](../resources/groupsettingtemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4ca96-118">If successful, this method returns a `200 OK` response code and [groupSettingTemplate](../resources/groupsettingtemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ca96-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4ca96-119">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4ca96-120">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4ca96-120">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groupsettingtemplate"
}-->
```http
GET https://graph.microsoft.com/v1.0/groupSettingTemplates/{id}
```
##### <a name="response"></a><span data-ttu-id="4ca96-121">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ca96-121">Response</span></span>

<span data-ttu-id="4ca96-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4ca96-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSettingTemplate"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1341

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groupSettingTemplates/$entity",
    "id": "62375ab9-6b52-47ed-826b-58e47e0e304b",
    "deletedDateTime": null,
    "displayName": "Group.Unified",
    "description": "Setting templates define the different settings that can be used for the associated ObjectSettings. This template defines settings that can be used for Unified Groups.",
    "values": [
        {
            "name": "CustomBlockedWordsList",
            "type": "System.String",
            "defaultValue": "",
            "description": "A comma-delimited list of blocked words for Unified Group displayName and mailNickName."
        },
        {
            "name": "EnableMSStandardBlockedWords",
            "type": "System.Boolean",
            "defaultValue": "false",
            "description": "A flag indicating whether or not to enable the Microsoft Standard list of blocked words for Unified Group displayName and mailNickName."
        },
        {
            "name": "ClassificationDescriptions",
            "type": "System.String",
            "defaultValue": "",
            "description": "A comma-delimited list of structured strings describing the classification values in the ClassificationList. The structure of the string is: Value: Description"
        }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get groupSettingTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->