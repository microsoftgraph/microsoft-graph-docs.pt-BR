# <a name="delete-calendargroup"></a><span data-ttu-id="8dee7-101">Excluir calendarGroup</span><span class="sxs-lookup"><span data-stu-id="8dee7-101">Delete calendarGroup</span></span>

<span data-ttu-id="8dee7-102">Exclui um grupo de calendários diferente do grupo de calendários padrão.</span><span class="sxs-lookup"><span data-stu-id="8dee7-102">Delete a calendar group other than the default calendar group.</span></span>

<span data-ttu-id="8dee7-p101">**Observação** O Outlook.com oferece suporte somente ao grupo de calendários padrão que pode ser acessado pelo atalho /me/calendars. Você não pode excluir nenhum grupo de calendários no Outlook.com.</span><span class="sxs-lookup"><span data-stu-id="8dee7-p101">**Note** Outlook.com supports only the default calendar group which is accessible by the /me/calendars shortcut. You cannot delete any calendar group in Outlook.com.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8dee7-105">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8dee7-105">Prerequisites</span></span>
<span data-ttu-id="8dee7-106">Um dos seguintes **escopos** é necessário para executar esta API: *Calendars.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="8dee7-106">One of the following **scopes** is required to execute this API: *Calendars.ReadWrite*</span></span>
## <a name="http-request"></a><span data-ttu-id="8dee7-107">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8dee7-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/calendarGroups/{id}
DELETE /users/{id | userPrincipalName}/calendarGroups/{id}
```
## <a name="request-headers"></a><span data-ttu-id="8dee7-108">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8dee7-108">Request headers</span></span>
| <span data-ttu-id="8dee7-109">Nome</span><span class="sxs-lookup"><span data-stu-id="8dee7-109">Name</span></span>       | <span data-ttu-id="8dee7-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="8dee7-110">Type</span></span> | <span data-ttu-id="8dee7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8dee7-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8dee7-112">Autorização</span><span class="sxs-lookup"><span data-stu-id="8dee7-112">Authorization</span></span>  | <span data-ttu-id="8dee7-113">string</span><span class="sxs-lookup"><span data-stu-id="8dee7-113">string</span></span>  | <span data-ttu-id="8dee7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8dee7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8dee7-116">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8dee7-116">Request body</span></span>
<span data-ttu-id="8dee7-117">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8dee7-117">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8dee7-118">Resposta</span><span class="sxs-lookup"><span data-stu-id="8dee7-118">Response</span></span>

<span data-ttu-id="8dee7-p103">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8dee7-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8dee7-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8dee7-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8dee7-122">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8dee7-122">Request</span></span>
<span data-ttu-id="8dee7-123">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8dee7-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_calendargroup"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/calendarGroups/{id}
```
##### <a name="response"></a><span data-ttu-id="8dee7-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="8dee7-124">Response</span></span>
<span data-ttu-id="8dee7-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8dee7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete calendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
