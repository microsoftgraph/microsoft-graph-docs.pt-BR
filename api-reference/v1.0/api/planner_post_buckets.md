# <a name="create-plannerbucket"></a><span data-ttu-id="035b6-101">Criar plannerBucket</span><span class="sxs-lookup"><span data-stu-id="035b6-101">Create plannerBucket</span></span>

<span data-ttu-id="035b6-102">Use essa API para criar um novo **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="035b6-102">Use this API to create a new **plannerBucket**.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="035b6-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="035b6-103">Prerequisites</span></span>
<span data-ttu-id="035b6-104">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="035b6-104">The following **scopes** are required to execute this API:</span></span> 

<span data-ttu-id="035b6-105">*Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="035b6-105">*Group.ReadWrite.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="035b6-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="035b6-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /planner/buckets

```
## <a name="request-headers"></a><span data-ttu-id="035b6-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="035b6-107">Request headers</span></span>
| <span data-ttu-id="035b6-108">Nome</span><span class="sxs-lookup"><span data-stu-id="035b6-108">Name</span></span>       | <span data-ttu-id="035b6-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="035b6-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="035b6-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="035b6-110">Authorization</span></span>  | <span data-ttu-id="035b6-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="035b6-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="035b6-113">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="035b6-113">Request body</span></span>
<span data-ttu-id="035b6-114">No corpo da solicitação, forneça uma representação JSON do objeto [plannerBucket](../resources/plannerbucket.md).</span><span class="sxs-lookup"><span data-stu-id="035b6-114">In the request body, supply a JSON representation of [plannerBucket](../resources/plannerbucket.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="035b6-115">Resposta</span><span class="sxs-lookup"><span data-stu-id="035b6-115">Response</span></span>

<span data-ttu-id="035b6-116">Se bem-sucedido, este método retorna o código de resposta `201, Created` e o objeto [plannerBucket](../resources/plannerbucket.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="035b6-116">If successful, this method returns `201, Created` response code and [plannerBucket](../resources/plannerbucket.md) object in the response body.</span></span>

<span data-ttu-id="035b6-p102">Este método pode retornar qualquer um dos [códigos de status de HTTP](../../../concepts/errors.md). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403 e 404. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner_overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="035b6-p102">This method can return any of the [HTTP status codes](../../../concepts/errors.md). The most common errors that apps should handle for this method are the 400, 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner_overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="035b6-120">Exemplo</span><span class="sxs-lookup"><span data-stu-id="035b6-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="035b6-121">Solicitação</span><span class="sxs-lookup"><span data-stu-id="035b6-121">Request</span></span>
<span data-ttu-id="035b6-122">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="035b6-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_plannerbucket_from_planner"
}-->
```http
POST https://graph.microsoft.com/v1.0/planner/buckets
Content-type: application/json
Content-length: 92

{
  "name": "Advertising",
  "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
  "orderHint": " !"
}
```
<span data-ttu-id="035b6-123">No corpo da solicitação, forneça uma representação JSON do objeto [plannerBucket](../resources/plannerbucket.md).</span><span class="sxs-lookup"><span data-stu-id="035b6-123">In the request body, supply a JSON representation of [plannerBucket](../resources/plannerbucket.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="035b6-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="035b6-124">Response</span></span>
<span data-ttu-id="035b6-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="035b6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucket"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 145

{
  "name": "Advertising",
  "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
  "orderHint": "85752723360752+",
  "id": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create plannerBucket",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->