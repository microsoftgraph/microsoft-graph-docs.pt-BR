---
title: Criar accessReviewHistoryDefinition
description: Crie um novo objeto accessReviewHistoryDefinition.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: f266276fae151bd8cc31455c4fd69eab193dd440
ms.sourcegitcommit: 276a13a37c3772689dfc71f7cd47586c9581f27d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/24/2021
ms.locfileid: "52629218"
---
# <a name="create-accessreviewhistorydefinition"></a><span data-ttu-id="1b100-103">Criar accessReviewHistoryDefinition</span><span class="sxs-lookup"><span data-stu-id="1b100-103">Create accessReviewHistoryDefinition</span></span>

<span data-ttu-id="1b100-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b100-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b100-105">Crie um novo [objeto accessReviewHistoryDefinition.](../resources/accessreviewhistorydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="1b100-105">Create a new [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1b100-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="1b100-106">Permissions</span></span>

<span data-ttu-id="1b100-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b100-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b100-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1b100-109">Permission type</span></span>|<span data-ttu-id="1b100-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1b100-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1b100-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1b100-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1b100-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b100-112">AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="1b100-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1b100-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1b100-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1b100-114">Not supported.</span></span>|
|<span data-ttu-id="1b100-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1b100-115">Application</span></span>|<span data-ttu-id="1b100-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b100-116">AccessReview.ReadWrite.All</span></span>|

<span data-ttu-id="1b100-117">O usuário de entrada também deve estar em uma função de diretório que permita que ele leia uma revisão de acesso para recuperar todos os dados.</span><span class="sxs-lookup"><span data-stu-id="1b100-117">The signed-in user must also be in a directory role that permits them to read an access review to retrieve any data.</span></span>  <span data-ttu-id="1b100-118">Para obter mais detalhes, consulte os requisitos de função e permissão para [avaliações de acesso.](../resources/accessreviewsv2-root.md)</span><span class="sxs-lookup"><span data-stu-id="1b100-118">For more details, see the role and permission requirements for [access reviews](../resources/accessreviewsv2-root.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="1b100-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1b100-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/accessReviews/historyDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="1b100-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1b100-120">Request headers</span></span>

|<span data-ttu-id="1b100-121">Nome</span><span class="sxs-lookup"><span data-stu-id="1b100-121">Name</span></span>|<span data-ttu-id="1b100-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b100-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1b100-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1b100-123">Authorization</span></span>|<span data-ttu-id="1b100-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1b100-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="1b100-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1b100-126">Content-Type</span></span>|<span data-ttu-id="1b100-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1b100-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b100-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1b100-129">Request body</span></span>

<span data-ttu-id="1b100-130">No corpo da solicitação, fornece uma representação JSON do [objeto accessReviewHistoryDefinition.](../resources/accessreviewhistorydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="1b100-130">In the request body, supply a JSON representation of the [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) object.</span></span>

<span data-ttu-id="1b100-131">A tabela a seguir mostra as propriedades necessárias usadas para criar [um accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md).</span><span class="sxs-lookup"><span data-stu-id="1b100-131">The following table shows the required properties used to create an [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md).</span></span>

|<span data-ttu-id="1b100-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1b100-132">Property</span></span>|<span data-ttu-id="1b100-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="1b100-133">Type</span></span>|<span data-ttu-id="1b100-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b100-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b100-135">displayName</span><span class="sxs-lookup"><span data-stu-id="1b100-135">displayName</span></span> | <span data-ttu-id="1b100-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b100-136">String</span></span>  | <span data-ttu-id="1b100-137">Nome da coleção de dados do histórico de revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="1b100-137">Name for the access review history data collection.</span></span> <span data-ttu-id="1b100-138">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1b100-138">Required.</span></span> |
|<span data-ttu-id="1b100-139">reviewHistoryPeriodStartDateTime</span><span class="sxs-lookup"><span data-stu-id="1b100-139">reviewHistoryPeriodStartDateTime</span></span>  | <span data-ttu-id="1b100-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b100-140">DateTimeOffset</span></span>  | <span data-ttu-id="1b100-141">Timestamp, as avaliações que começam em ou após essa data serão incluídas nos dados de histórico buscados.</span><span class="sxs-lookup"><span data-stu-id="1b100-141">Timestamp, reviews starting on or after this date will be included in the fetched history data.</span></span> <span data-ttu-id="1b100-142">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1b100-142">Required.</span></span>  |
|<span data-ttu-id="1b100-143">reviewHistoryPeriodEndDateTime</span><span class="sxs-lookup"><span data-stu-id="1b100-143">reviewHistoryPeriodEndDateTime</span></span>  | <span data-ttu-id="1b100-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b100-144">DateTimeOffset</span></span>  | <span data-ttu-id="1b100-145">Timestamp, as avaliações que começam em ou antes dessa data serão incluídas nos dados de histórico buscados.</span><span class="sxs-lookup"><span data-stu-id="1b100-145">Timestamp, reviews starting on or before this date will be included in the fetched history data.</span></span> <span data-ttu-id="1b100-146">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1b100-146">Required.</span></span>  |
|<span data-ttu-id="1b100-147">escopos</span><span class="sxs-lookup"><span data-stu-id="1b100-147">scopes</span></span>|<span data-ttu-id="1b100-148">[Coleção accessReviewQueryScope](../resources/accessreviewqueryscope.md)</span><span class="sxs-lookup"><span data-stu-id="1b100-148">[accessReviewQueryScope](../resources/accessreviewqueryscope.md) collection</span></span>| <span data-ttu-id="1b100-149">Usado para filtrar quais avaliações estão incluídas nos dados de histórico buscados.</span><span class="sxs-lookup"><span data-stu-id="1b100-149">Used to filter which reviews are included in the fetched history data.</span></span> <span data-ttu-id="1b100-150">Busca avaliações cujo escopo corresponde a esse escopo fornecido.</span><span class="sxs-lookup"><span data-stu-id="1b100-150">Fetches reviews whose scope matches with this provided scope.</span></span> <span data-ttu-id="1b100-151">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1b100-151">Required.</span></span> <br> <span data-ttu-id="1b100-152">Para obter mais, consulte Consultas de escopo com [suporte para accessReviewHistoryDefinition](#supported-scope-queries-for-accessreviewhistorydefinition).</span><span class="sxs-lookup"><span data-stu-id="1b100-152">For more, see [Supported scope queries for accessReviewHistoryDefinition](#supported-scope-queries-for-accessreviewhistorydefinition).</span></span> |

### <a name="supported-scope-queries-for-accessreviewhistorydefinition"></a><span data-ttu-id="1b100-153">Consultas de escopo com suporte para accessReviewHistoryDefinition</span><span class="sxs-lookup"><span data-stu-id="1b100-153">Supported scope queries for accessReviewHistoryDefinition</span></span>

<span data-ttu-id="1b100-154">A **propriedade scopes** [de accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) baseia-se no **accessReviewQueryScope**, um recurso que permite configurar diferentes recursos em sua propriedade de **consulta.**</span><span class="sxs-lookup"><span data-stu-id="1b100-154">The **scopes** property of [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) is based on **accessReviewQueryScope**, a resource that allows you to configure different resources in it's **query** property.</span></span> <span data-ttu-id="1b100-155">Esses recursos representam o escopo da definição de histórico e ditam o tipo de dados de histórico de revisão incluídos no arquivo CSV baixável que é gerado quando a definição de histórico é criada.</span><span class="sxs-lookup"><span data-stu-id="1b100-155">These resources then represent the scope of the history definition and dictate the type of review history data that is included in the downloadable CSV file which is generated when the history definition is created.</span></span>

<span data-ttu-id="1b100-156">Use o seguinte formato para **a propriedade de** consulta:</span><span class="sxs-lookup"><span data-stu-id="1b100-156">Use the following format for the **query** property:</span></span>

```http
/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '{object}')
```

<span data-ttu-id="1b100-157">O valor `{object}` de é um dos recursos que podem ser configurados em um **accessReviewScheduleDefinition**.</span><span class="sxs-lookup"><span data-stu-id="1b100-157">The value of `{object}` is one of the resources that can be configured in an **accessReviewScheduleDefinition**.</span></span> <span data-ttu-id="1b100-158">Por exemplo, o seguinte inclui todos os resultados de revisão accessReviewScheduleDefinition em grupos individuais (e exclui definições com escopo para todos os grupos Microsoft 365 com usuários convidados).</span><span class="sxs-lookup"><span data-stu-id="1b100-158">For example, the following includes every accessReviewScheduleDefinition review result on individual groups (and excludes definitions scoped to all Microsoft 365 groups with guest users).</span></span>

```http
/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '/groups')
```

<span data-ttu-id="1b100-159">Para obter valores mais suportados, consulte Use o parâmetro $filter de consulta [no accessReviewScheduleDefinition](accessreviewscheduledefinition-list.md#use-the-filter-query-parameter).</span><span class="sxs-lookup"><span data-stu-id="1b100-159">For more supported values, see Use the [$filter query parameter on accessReviewScheduleDefinition](accessreviewscheduledefinition-list.md#use-the-filter-query-parameter).</span></span>

## <a name="response"></a><span data-ttu-id="1b100-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b100-160">Response</span></span>

<span data-ttu-id="1b100-161">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1b100-161">If successful, this method returns a `201 Created` response code and an [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1b100-162">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1b100-162">Examples</span></span>

<span data-ttu-id="1b100-163">O exemplo a seguir mostra como criar uma definição de histórico de revisão de acesso com escopo para acessar análises em pacotes e grupos de acesso, em execução entre a data de início de 01/01/2021 e a data de término de 05/04/2021.</span><span class="sxs-lookup"><span data-stu-id="1b100-163">The following example shows how to create an access review history definition scoped to access reviews on access packages and groups, running between the start date of 01/01/2021 and end date of 04/05/2021.</span></span>

### <a name="request"></a><span data-ttu-id="1b100-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1b100-164">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="1b100-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="1b100-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accessreviewhistorydefinition_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/historyDefinitions
Content-Type: application/json

{
  "displayName": "Last quarter's group reviews April 2021",
  "decisions": [
    "approve",
    "deny",
    "dontKnow",
    "notReviewed",
    "notNotified"
  ],
  "reviewHistoryPeriodStartDateTime": "2021-01-01T00:00:00Z",
  "reviewHistoryPeriodEndDateTime": "2021-04-05T00:00:00Z",
  "scopes": [
    {
      "@odata.type": "#microsoft.graph.accessReviewQueryScope",
      "queryType": "MicrosoftGraph",     
      "query": "/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, 'accessPackageAssignments')",
      "queryRoot": null
    },  
    {
      "@odata.type": "#microsoft.graph.accessReviewQueryScope",
      "queryType": "MicrosoftGraph",     
      "query": "/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '/groups')",
      "queryRoot": null
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="1b100-166">C#</span><span class="sxs-lookup"><span data-stu-id="1b100-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accessreviewhistorydefinition-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1b100-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1b100-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accessreviewhistorydefinition-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1b100-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1b100-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accessreviewhistorydefinition-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1b100-169">Java</span><span class="sxs-lookup"><span data-stu-id="1b100-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accessreviewhistorydefinition-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="1b100-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b100-170">Response</span></span>
><span data-ttu-id="1b100-171">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1b100-171">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewHistoryDefinition"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.accessReviewHistoryDefinition",
  "id": "b2cb022f-b7e1-40f3-9854-c65a40861c38",
  "displayName": "Last quarter's group reviews April 2021",
  "reviewHistoryPeriodStartDateTime": "2021-01-01T00:00:00Z",
  "reviewHistoryPeriodEndDateTime": "2021-04-05T00:00:00Z",
  "decisions": [
    "approve",
    "deny",
    "dontKnow",
    "notReviewed",
    "notNotified"
  ],
  "status": "requested",
  "createdDateTime": "2021-04-14T00:22:48.9392594Z",
  "fulfilledDateTime": null,
  "downloadUri": null,
  "createdBy": {
      "id": "957f1027-c0ee-460d-9269-b8444459e0fe",
      "displayName": "MOD Administrator",
      "userPrincipalName": "admin@contoso.com"
  },
  "scopes": [
    {
      "@odata.type": "#microsoft.graph.accessReviewQueryScope",
      "queryType": "MicrosoftGraph",     
      "query": "/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, 'accessPackageAssignments')",
      "queryRoot": null
    },  
    {
      "@odata.type": "#microsoft.graph.accessReviewQueryScope",
      "queryType": "MicrosoftGraph",     
      "query": "/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '/groups')",
      "queryRoot": null
    }
  ]
}
```
