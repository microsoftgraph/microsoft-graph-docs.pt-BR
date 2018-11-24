# <a name="get-a-group-setting-template"></a><span data-ttu-id="5d301-101">Obter um modelo de configuração de grupo</span><span class="sxs-lookup"><span data-stu-id="5d301-101">Get a group setting template</span></span>

<span data-ttu-id="5d301-p101">Um modelo de configuração de grupo representa um modelo de configurações pelo qual as configurações podem ser criadas dentro de um locatário. Esta operação permite recuperação das propriedades do objeto [groupSettingTemplate](../resources/groupsettingtemplate.md), inclusive as configurações disponíveis e seus padrões.</span><span class="sxs-lookup"><span data-stu-id="5d301-p101">A group setting template represents a template of settings from which settings may be created within a tenant. This operation allows retrieval of the properties of the [groupSettingTemplate](../resources/groupsettingtemplate.md) object, including the available settings and their defaults.</span></span>

## <a name="permissions"></a><span data-ttu-id="5d301-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="5d301-104">Permissions</span></span>

<span data-ttu-id="5d301-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5d301-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="5d301-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5d301-107">Permission type</span></span>      | <span data-ttu-id="5d301-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5d301-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5d301-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5d301-109">Delegated (work or school account)</span></span> | <span data-ttu-id="5d301-110">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5d301-110">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5d301-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5d301-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d301-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5d301-112">Not supported.</span></span>    |
|<span data-ttu-id="5d301-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5d301-113">Application</span></span> | <span data-ttu-id="5d301-114">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d301-114">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5d301-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5d301-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupSettingTemplates/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5d301-116">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5d301-116">Optional query parameters</span></span>
<span data-ttu-id="5d301-117">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5d301-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5d301-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5d301-118">Request headers</span></span>
| <span data-ttu-id="5d301-119">Nome</span><span class="sxs-lookup"><span data-stu-id="5d301-119">Name</span></span> | <span data-ttu-id="5d301-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d301-120">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="5d301-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5d301-121">Authorization</span></span> | <span data-ttu-id="5d301-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5d301-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5d301-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5d301-124">Request body</span></span>
<span data-ttu-id="5d301-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5d301-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5d301-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d301-126">Response</span></span>

<span data-ttu-id="5d301-127">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [groupSettingTemplate](../resources/groupsettingtemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5d301-127">If successful, this method returns a `200 OK` response code and [groupSettingTemplate](../resources/groupsettingtemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d301-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5d301-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5d301-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5d301-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groupsettingtemplate"
}-->
```http
GET https://graph.microsoft.com/v1.0/groupSettingTemplates/{id}
```
##### <a name="response"></a><span data-ttu-id="5d301-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d301-130">Response</span></span>

<span data-ttu-id="5d301-p104">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5d301-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    ]
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