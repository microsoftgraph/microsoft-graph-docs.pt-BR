---
title: Atualizar aplicativo
description: Atualiza as propriedades do objeto Application.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c184a7f51f67519f76c39c7f44d1f9a39368c4db
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258412"
---
# <a name="update-application"></a><span data-ttu-id="496c1-103">Atualizar aplicativo</span><span class="sxs-lookup"><span data-stu-id="496c1-103">Update application</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="496c1-104">Atualiza as propriedades do objeto Application.</span><span class="sxs-lookup"><span data-stu-id="496c1-104">Update the properties of application object.</span></span>
## <a name="permissions"></a><span data-ttu-id="496c1-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="496c1-105">Permissions</span></span>
<span data-ttu-id="496c1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="496c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="496c1-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="496c1-108">Permission type</span></span>      | <span data-ttu-id="496c1-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="496c1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="496c1-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="496c1-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="496c1-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="496c1-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="496c1-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="496c1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="496c1-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="496c1-113">Not supported.</span></span>    |
|<span data-ttu-id="496c1-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="496c1-114">Application</span></span> | <span data-ttu-id="496c1-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="496c1-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="496c1-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="496c1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /applications/{id}
```
## <a name="request-headers"></a><span data-ttu-id="496c1-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="496c1-117">Request headers</span></span>
| <span data-ttu-id="496c1-118">Nome</span><span class="sxs-lookup"><span data-stu-id="496c1-118">Name</span></span>       | <span data-ttu-id="496c1-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="496c1-119">Type</span></span> | <span data-ttu-id="496c1-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="496c1-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="496c1-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="496c1-121">Authorization</span></span>  | <span data-ttu-id="496c1-122">string</span><span class="sxs-lookup"><span data-stu-id="496c1-122">string</span></span>  | <span data-ttu-id="496c1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="496c1-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="496c1-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="496c1-125">Request body</span></span>
<span data-ttu-id="496c1-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="496c1-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="496c1-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="496c1-129">Property</span></span>     | <span data-ttu-id="496c1-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="496c1-130">Type</span></span>   |<span data-ttu-id="496c1-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="496c1-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="496c1-132">Allowpublicclient e</span><span class="sxs-lookup"><span data-stu-id="496c1-132">allowPublicClient</span></span>|<span data-ttu-id="496c1-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="496c1-133">Boolean</span></span>| <span data-ttu-id="496c1-134">Especifica se o aplicativo pode atuar como um cliente público.</span><span class="sxs-lookup"><span data-stu-id="496c1-134">Specifies if the application can act as a public client.</span></span> <span data-ttu-id="496c1-135">Por exemplo, um aplicativo instalado em execução em um dispositivo móvel.</span><span class="sxs-lookup"><span data-stu-id="496c1-135">For example,  an installed application running on a mobile device.</span></span> <span data-ttu-id="496c1-136">O valor padrão é *false*.</span><span class="sxs-lookup"><span data-stu-id="496c1-136">Default value is *false*.</span></span> |
|<span data-ttu-id="496c1-137">api</span><span class="sxs-lookup"><span data-stu-id="496c1-137">api</span></span>|[<span data-ttu-id="496c1-138">apiApplication</span><span class="sxs-lookup"><span data-stu-id="496c1-138">apiApplication</span></span>](../resources/apiapplication.md)| <span data-ttu-id="496c1-139">Especifica configurações para um aplicativo de API.</span><span class="sxs-lookup"><span data-stu-id="496c1-139">Specifies settings for an API application.</span></span> |
|<span data-ttu-id="496c1-140">appRoles</span><span class="sxs-lookup"><span data-stu-id="496c1-140">appRoles</span></span>|<span data-ttu-id="496c1-141">Coleção [appRole](../resources/approle.md)</span><span class="sxs-lookup"><span data-stu-id="496c1-141">[appRole](../resources/approle.md) collection</span></span>|<span data-ttu-id="496c1-142">A coleção de funções de aplicativo que um aplicativo pode declarar.</span><span class="sxs-lookup"><span data-stu-id="496c1-142">The collection of application roles that an application may declare.</span></span> <span data-ttu-id="496c1-143">Essas funções podem ser atribuídas a usuários, grupos ou entidades de serviço.</span><span class="sxs-lookup"><span data-stu-id="496c1-143">These roles can be assigned to users, groups, or service principals.</span></span> <span data-ttu-id="496c1-144">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="496c1-144">Not nullable.</span></span>|
|<span data-ttu-id="496c1-145">É applicationaliases</span><span class="sxs-lookup"><span data-stu-id="496c1-145">applicationAliases</span></span>|<span data-ttu-id="496c1-146">Coleção String</span><span class="sxs-lookup"><span data-stu-id="496c1-146">String collection</span></span>| <span data-ttu-id="496c1-147">Os URIs que identificam o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="496c1-147">The URIs that identify the application.</span></span> <span data-ttu-id="496c1-148">Para saber mais, confira [Objetos do aplicativo e objetos da entidade de serviço](https://azure.microsoft.com/documentation/articles/active-directory-application-objects/).</span><span class="sxs-lookup"><span data-stu-id="496c1-148">For more information see, [Application Objects and Service Principal Objects](https://azure.microsoft.com/documentation/articles/active-directory-application-objects/).</span></span> <span data-ttu-id="496c1-149">O operador *any* é obrigatório para expressões de filtro em propriedades de vários valores.</span><span class="sxs-lookup"><span data-stu-id="496c1-149">The *any* operator is required for filter expressions on multi-valued properties.</span></span> <span data-ttu-id="496c1-150">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="496c1-150">Not nullable.</span></span> |
|<span data-ttu-id="496c1-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="496c1-151">createdDateTime</span></span>|<span data-ttu-id="496c1-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="496c1-152">DateTimeOffset</span></span>| <span data-ttu-id="496c1-153">A data e a hora que o aplicativo foi registrado.</span><span class="sxs-lookup"><span data-stu-id="496c1-153">The date and time the application was registered.</span></span> |
|<span data-ttu-id="496c1-154">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="496c1-154">deletedDateTime</span></span>|<span data-ttu-id="496c1-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="496c1-155">DateTimeOffset</span></span>| <span data-ttu-id="496c1-156">A data e a hora que o aplicativo foi excluído.</span><span class="sxs-lookup"><span data-stu-id="496c1-156">The date and time the application was deleted.</span></span> |
|<span data-ttu-id="496c1-157">displayName</span><span class="sxs-lookup"><span data-stu-id="496c1-157">displayName</span></span>|<span data-ttu-id="496c1-158">String</span><span class="sxs-lookup"><span data-stu-id="496c1-158">String</span></span>|<span data-ttu-id="496c1-159">O nome de exibição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="496c1-159">The display name for the application.</span></span> |
|<span data-ttu-id="496c1-160">id</span><span class="sxs-lookup"><span data-stu-id="496c1-160">id</span></span>|<span data-ttu-id="496c1-161">String</span><span class="sxs-lookup"><span data-stu-id="496c1-161">String</span></span>|<span data-ttu-id="496c1-162">O identificador exclusivo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="496c1-162">The unique identifier for the application.</span></span> <span data-ttu-id="496c1-163">Herdado de [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="496c1-163">Inherited from [directoryObject](../resources/directoryobject.md).</span></span> <span data-ttu-id="496c1-164">Chave.</span><span class="sxs-lookup"><span data-stu-id="496c1-164">Key.</span></span> <span data-ttu-id="496c1-165">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="496c1-165">Not nullable.</span></span> <span data-ttu-id="496c1-166">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="496c1-166">Read-only.</span></span> |
|<span data-ttu-id="496c1-167">informações </span><span class="sxs-lookup"><span data-stu-id="496c1-167">info</span></span>|[<span data-ttu-id="496c1-168">informationalUrl</span><span class="sxs-lookup"><span data-stu-id="496c1-168">informationalUrl</span></span>](../resources/informationalurl.md)| <span data-ttu-id="496c1-169">Informações de perfil básicas do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="496c1-169">Basic profile information of the application.</span></span> | <span data-ttu-id="496c1-170">Especifica configurações para clientes instalados, como dispositivos móveis ou da área de trabalho.</span><span class="sxs-lookup"><span data-stu-id="496c1-170">Specifies settings for installed clients such as desktop or mobile devices.</span></span> |
|<span data-ttu-id="496c1-171">keyCredentials</span><span class="sxs-lookup"><span data-stu-id="496c1-171">keyCredentials</span></span>|<span data-ttu-id="496c1-172">Coleção [keyCredential](../resources/keycredential.md)</span><span class="sxs-lookup"><span data-stu-id="496c1-172">[keyCredential](../resources/keycredential.md) collection</span></span>|<span data-ttu-id="496c1-173">A coleção de credenciais chaves associada ao aplicativo Não anulável.</span><span class="sxs-lookup"><span data-stu-id="496c1-173">The collection of key credentials associated with the application Not nullable.</span></span> |
|<span data-ttu-id="496c1-174">logo</span><span class="sxs-lookup"><span data-stu-id="496c1-174">logo</span></span>|<span data-ttu-id="496c1-175">Stream</span><span class="sxs-lookup"><span data-stu-id="496c1-175">Stream</span></span>|<span data-ttu-id="496c1-176">O principal logotipo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="496c1-176">The main logo for the application.</span></span> <span data-ttu-id="496c1-177">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="496c1-177">Not nullable.</span></span> |
|<span data-ttu-id="496c1-178">orgRestrictions</span><span class="sxs-lookup"><span data-stu-id="496c1-178">orgRestrictions</span></span>|<span data-ttu-id="496c1-179">Coleção String</span><span class="sxs-lookup"><span data-stu-id="496c1-179">String collection</span></span>| <span data-ttu-id="496c1-180">A organização tenantIds à qual o aplicativo é restrito.</span><span class="sxs-lookup"><span data-stu-id="496c1-180">The organizational tenantIds to which the application is restricted.</span></span>  <span data-ttu-id="496c1-181">Se a coleção estiver vazia, o aplicativo será multilocatário (não restrito).</span><span class="sxs-lookup"><span data-stu-id="496c1-181">If the collection is empty, the application is multi-tenant (not restricted).</span></span> <span data-ttu-id="496c1-182">Se a coleção contiver tenantIds, o aplicativo será restrito ao tenantIds organizacional na coleção.</span><span class="sxs-lookup"><span data-stu-id="496c1-182">If the collection contains tenantIds, the application is restricted to the organizational tenantIds in the collection.</span></span> <span data-ttu-id="496c1-183">A especificação de outros locatários, mas não o tenantid onde o aplicativo está registrado indica que a própria tenantid do aplicativo está indiretamente incluída.</span><span class="sxs-lookup"><span data-stu-id="496c1-183">Specifying other tenants but not the tenantId where the application is registered implies that the application's own tenantId is indirectly included.</span></span> |
|<span data-ttu-id="496c1-184">passwordCredentials</span><span class="sxs-lookup"><span data-stu-id="496c1-184">passwordCredentials</span></span>|<span data-ttu-id="496c1-185">Coleção [passwordCredential](../resources/passwordcredential.md)</span><span class="sxs-lookup"><span data-stu-id="496c1-185">[passwordCredential](../resources/passwordcredential.md) collection</span></span>|<span data-ttu-id="496c1-186">A coleção de credenciais de senha associada ao aplicativo.</span><span class="sxs-lookup"><span data-stu-id="496c1-186">The collection of password credentials associated with the application.</span></span> <span data-ttu-id="496c1-187">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="496c1-187">Not nullable.</span></span>|
|<span data-ttu-id="496c1-188">preAuthorizedApplications</span><span class="sxs-lookup"><span data-stu-id="496c1-188">preAuthorizedApplications</span></span>|<span data-ttu-id="496c1-189">coleção [preauthorizedapplication e](../resources/preauthorizedapplication.md)</span><span class="sxs-lookup"><span data-stu-id="496c1-189">[preAuthorizedApplication](../resources/preauthorizedapplication.md) collection</span></span>| <span data-ttu-id="496c1-190">Lista os aplicativos e as permissões solicitadas para o consentimento implícito.</span><span class="sxs-lookup"><span data-stu-id="496c1-190">Lists applications and requested permissions for implicit consent.</span></span> <span data-ttu-id="496c1-191">Requer um administrador para ter fornecido o consentimento para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="496c1-191">Requires an admin to have provided consent to the application.</span></span> <span data-ttu-id="496c1-192">o preAuthorizedApplications não exige que o usuário concorde com as permissões solicitadas.</span><span class="sxs-lookup"><span data-stu-id="496c1-192">preAuthorizedApplications do not require the user to consent to the requested permissions.</span></span> <span data-ttu-id="496c1-193">As permissões listadas no preAuthorizedApplications não exigem o consentimento do usuário.</span><span class="sxs-lookup"><span data-stu-id="496c1-193">Permissions listed in preAuthorizedApplications do not require user consent.</span></span> <span data-ttu-id="496c1-194">No entanto, as permissões adicionais solicitadas não listadas no preAuthorizedApplications exigem o consentimento do usuário.</span><span class="sxs-lookup"><span data-stu-id="496c1-194">However, any additional requested permissions not listed in preAuthorizedApplications require user consent.</span></span> |
|<span data-ttu-id="496c1-195">requiredResourceAccess</span><span class="sxs-lookup"><span data-stu-id="496c1-195">requiredResourceAccess</span></span>|<span data-ttu-id="496c1-196">[requiredResourceAccess](../resources/requiredresourceaccess.md) collection</span><span class="sxs-lookup"><span data-stu-id="496c1-196">[requiredResourceAccess](../resources/requiredresourceaccess.md) collection</span></span>|<span data-ttu-id="496c1-197">Especifica os recursos para os quais esse aplicativo requer acesso e o conjunto de escopos de permissão e funções de aplicativo do OAuth necessários em cada um desses recursos.</span><span class="sxs-lookup"><span data-stu-id="496c1-197">Specifies resources that this application requires access to and the set of OAuth permission scopes and application roles that it needs under each of those resources.</span></span> <span data-ttu-id="496c1-198">Essa pré-configuração de acesso necessário aos recursos impulsiona a experiência de consentimento.</span><span class="sxs-lookup"><span data-stu-id="496c1-198">This pre-configuration of required resource access drives the consent experience.</span></span> <span data-ttu-id="496c1-199">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="496c1-199">Not nullable.</span></span>|
|<span data-ttu-id="496c1-200">tags</span><span class="sxs-lookup"><span data-stu-id="496c1-200">tags</span></span>|<span data-ttu-id="496c1-201">Coleção String</span><span class="sxs-lookup"><span data-stu-id="496c1-201">String collection</span></span>| <span data-ttu-id="496c1-202">Sequências personalizadas que podem ser usadas para categorizar e identificar o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="496c1-202">Custom strings that can be used to categorize and identify the application.</span></span> |
|<span data-ttu-id="496c1-203">web</span><span class="sxs-lookup"><span data-stu-id="496c1-203">web</span></span>|[<span data-ttu-id="496c1-204">webApplication</span><span class="sxs-lookup"><span data-stu-id="496c1-204">webApplication</span></span>](../resources/webapplication.md)| <span data-ttu-id="496c1-205">Especifica configurações para um aplicativo Web.</span><span class="sxs-lookup"><span data-stu-id="496c1-205">Specifies settings for a web application.</span></span> |

## <a name="response"></a><span data-ttu-id="496c1-206">Resposta</span><span class="sxs-lookup"><span data-stu-id="496c1-206">Response</span></span>

<span data-ttu-id="496c1-207">Se tiver êxito, este método retornará `204 No Content` um código de resposta e não retornará nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="496c1-207">If successful, this method returns a `204 No Content` response code and does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="496c1-208">Exemplo</span><span class="sxs-lookup"><span data-stu-id="496c1-208">Example</span></span>
##### <a name="request"></a><span data-ttu-id="496c1-209">Solicitação</span><span class="sxs-lookup"><span data-stu-id="496c1-209">Request</span></span>
<span data-ttu-id="496c1-210">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="496c1-210">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_application"
}-->
```http
PATCH https://graph.microsoft.com/beta/applications/{id}
Content-type: application/json
Content-length: 72

{
  "allowPublicClient": false,
  "displayName": "New display name"
}
```
##### <a name="response"></a><span data-ttu-id="496c1-211">Resposta</span><span class="sxs-lookup"><span data-stu-id="496c1-211">Response</span></span>
<span data-ttu-id="496c1-212">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="496c1-212">Note: The response object shown here may be truncated for brevity.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="496c1-213">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="496c1-213">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="496c1-214">C#</span><span class="sxs-lookup"><span data-stu-id="496c1-214">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_application-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="496c1-215">Javascript</span><span class="sxs-lookup"><span data-stu-id="496c1-215">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_application-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="496c1-216">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="496c1-216">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_application-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update application",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/application-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/application-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/application-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
