# <a name="list-groupsettingtemplates"></a><span data-ttu-id="42bf2-101">Lista groupSettingTemplates</span><span class="sxs-lookup"><span data-stu-id="42bf2-101">List groupSettingTemplates</span></span>

<span data-ttu-id="42bf2-p101">Os Modelos de configuração de grupo representam um conjunto de modelos pelo qual as configurações de grupo podem ser criadas e usadas em um locatário.  Esta operação recupera a lista de objetos groupSettingTemplates disponíveis.</span><span class="sxs-lookup"><span data-stu-id="42bf2-p101">Group setting templates represents a set of templates  from which group settings may be created and used within a tenant.  This operation retrieves the list of available groupSettingTemplates objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="42bf2-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="42bf2-104">Prerequisites</span></span>

<span data-ttu-id="42bf2-105">Os seguintes **escopos** são necessários para executar esta API: *Directory.Read.All*, *Directory.ReadWrite.All* ou *Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="42bf2-105">The following **scopes** are required to execute this API: *Directory.Read.All* or *Directory.ReadWrite.All* or *Directory.AccessAsUser.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="42bf2-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="42bf2-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupSettingTemplates
```
## <a name="optional-query-parameters"></a><span data-ttu-id="42bf2-107">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="42bf2-107">Optional query parameters</span></span>
<span data-ttu-id="42bf2-108">Este método dá suporte a [Parâmetros de consulta OData](http://graph.microsoft.io/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="42bf2-108">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

> <span data-ttu-id="42bf2-109">**Observação:** $filter não é suportado.</span><span class="sxs-lookup"><span data-stu-id="42bf2-109">**Note:** $filter is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="42bf2-110">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="42bf2-110">Request headers</span></span>
| <span data-ttu-id="42bf2-111">Nome</span><span class="sxs-lookup"><span data-stu-id="42bf2-111">Name</span></span> | <span data-ttu-id="42bf2-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="42bf2-112">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="42bf2-113">Autorização</span><span class="sxs-lookup"><span data-stu-id="42bf2-113">Authorization</span></span>  | <span data-ttu-id="42bf2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="42bf2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="42bf2-116">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="42bf2-116">Request body</span></span>
<span data-ttu-id="42bf2-117">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="42bf2-117">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="42bf2-118">Resposta</span><span class="sxs-lookup"><span data-stu-id="42bf2-118">Response</span></span>

<span data-ttu-id="42bf2-119">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [groupSettingTemplate](../resources/groupsettingtemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="42bf2-119">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/groupsettingtemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42bf2-120">Exemplo</span><span class="sxs-lookup"><span data-stu-id="42bf2-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="42bf2-121">Solicitação</span><span class="sxs-lookup"><span data-stu-id="42bf2-121">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groupsettingtemplates"
}-->
```http
GET https://graph.microsoft.com/v1.0/groupSettingTemplates
```
##### <a name="response"></a><span data-ttu-id="42bf2-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="42bf2-122">Response</span></span>

<span data-ttu-id="42bf2-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="42bf2-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSettingTemplate",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1770

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groupSettingTemplates",
    "value": [
                {
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
            ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groupSettingTemplates",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->