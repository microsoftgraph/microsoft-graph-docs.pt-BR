---
title: Atualizar serviceprincipal
description: Atualize as propriedades do objeto serviceprincipal.
localization_priority: Normal
ms.openlocfilehash: 946db869863d74a94e2e9adc04a66c8d9a50e4f5
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573855"
---
# <a name="update-serviceprincipal"></a><span data-ttu-id="e5c94-103">Atualizar serviceprincipal</span><span class="sxs-lookup"><span data-stu-id="e5c94-103">Update serviceprincipal</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5c94-104">Atualize as propriedades do objeto serviceprincipal.</span><span class="sxs-lookup"><span data-stu-id="e5c94-104">Update the properties of serviceprincipal object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e5c94-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e5c94-105">Permissions</span></span>
<span data-ttu-id="e5c94-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5c94-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5c94-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e5c94-108">Permission type</span></span>      | <span data-ttu-id="e5c94-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e5c94-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e5c94-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e5c94-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e5c94-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e5c94-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e5c94-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e5c94-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5c94-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e5c94-113">Not supported.</span></span>    |
|<span data-ttu-id="e5c94-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5c94-114">Application</span></span> | <span data-ttu-id="e5c94-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5c94-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e5c94-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e5c94-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /servicePrincipals/{id}
```
## <a name="request-headers"></a><span data-ttu-id="e5c94-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e5c94-117">Request headers</span></span>
| <span data-ttu-id="e5c94-118">Nome</span><span class="sxs-lookup"><span data-stu-id="e5c94-118">Name</span></span>       | <span data-ttu-id="e5c94-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="e5c94-119">Type</span></span> | <span data-ttu-id="e5c94-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5c94-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e5c94-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e5c94-121">Authorization</span></span>  | <span data-ttu-id="e5c94-122">string</span><span class="sxs-lookup"><span data-stu-id="e5c94-122">string</span></span>  | <span data-ttu-id="e5c94-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e5c94-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e5c94-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e5c94-125">Request body</span></span>
<span data-ttu-id="e5c94-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="e5c94-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e5c94-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e5c94-129">Property</span></span>     | <span data-ttu-id="e5c94-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="e5c94-130">Type</span></span>   |<span data-ttu-id="e5c94-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5c94-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e5c94-132">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="e5c94-132">accountEnabled</span></span>|<span data-ttu-id="e5c94-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5c94-133">Boolean</span></span>|                <span data-ttu-id="e5c94-134">**true** se a conta de serviço principal estiver ativada; Caso contrário, **false**.</span><span class="sxs-lookup"><span data-stu-id="e5c94-134">**true** if the service principal account is enabled; otherwise, **false**.</span></span>            |
|<span data-ttu-id="e5c94-135">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="e5c94-135">appDisplayName</span></span>|<span data-ttu-id="e5c94-136">String</span><span class="sxs-lookup"><span data-stu-id="e5c94-136">String</span></span>|<span data-ttu-id="e5c94-137">O nome de exibição exposto pelo aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="e5c94-137">The display name exposed by the associated application.</span></span>|
|<span data-ttu-id="e5c94-138">appId</span><span class="sxs-lookup"><span data-stu-id="e5c94-138">appId</span></span>|<span data-ttu-id="e5c94-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e5c94-139">String</span></span>|<span data-ttu-id="e5c94-140">O identificador exclusivo para o aplicativo associado (sua propriedade **appId** ).</span><span class="sxs-lookup"><span data-stu-id="e5c94-140">The unique identifier for the associated application (its **appId** property).</span></span>|
|<span data-ttu-id="e5c94-141">appRoleAssignmentRequired</span><span class="sxs-lookup"><span data-stu-id="e5c94-141">appRoleAssignmentRequired</span></span>|<span data-ttu-id="e5c94-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5c94-142">Boolean</span></span>|<span data-ttu-id="e5c94-143">Especifica se um **appRoleAssignment** a um usuário ou grupo é necessária antes que o Azure AD emitirá um usuário ou um token de acesso ao aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e5c94-143">Specifies whether an **appRoleAssignment** to a user or group is required before Azure AD will issue a user or access token to the application.</span></span>                            <span data-ttu-id="e5c94-144">**Observações**: requer a versão 1.5 ou mais recente, não são nulas.</span><span class="sxs-lookup"><span data-stu-id="e5c94-144">**Notes**: Requires version 1.5 or newer, not nullable.</span></span>            |
|<span data-ttu-id="e5c94-145">appRoles</span><span class="sxs-lookup"><span data-stu-id="e5c94-145">appRoles</span></span>| <span data-ttu-id="e5c94-146">coleção [microsoft.graph.appRole](../resources/approle.md)</span><span class="sxs-lookup"><span data-stu-id="e5c94-146">[microsoft.graph.appRole](../resources/approle.md) collection</span></span>|<span data-ttu-id="e5c94-147">As funções do aplicativo expostas pelo aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="e5c94-147">The application roles exposed by the associated application.</span></span> <span data-ttu-id="e5c94-148">Para obter mais informações, consulte a definição da propriedade **appRoles** sobre a entidade de aplicativo **Notes**: requer a versão 1.5 ou mais recente, não são nulas.</span><span class="sxs-lookup"><span data-stu-id="e5c94-148">For more information see the **appRoles** property definition on the application entity                            **Notes**: Requires version 1.5 or newer, not nullable.</span></span>            |
|<span data-ttu-id="e5c94-149">displayName</span><span class="sxs-lookup"><span data-stu-id="e5c94-149">displayName</span></span>|<span data-ttu-id="e5c94-150">String</span><span class="sxs-lookup"><span data-stu-id="e5c94-150">String</span></span>|<span data-ttu-id="e5c94-151">O nome de exibição para a entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="e5c94-151">The display name for the service principal.</span></span>|
|<span data-ttu-id="e5c94-152">errorUrl</span><span class="sxs-lookup"><span data-stu-id="e5c94-152">errorUrl</span></span>|<span data-ttu-id="e5c94-153">String</span><span class="sxs-lookup"><span data-stu-id="e5c94-153">String</span></span>|            |
|<span data-ttu-id="e5c94-154">home page</span><span class="sxs-lookup"><span data-stu-id="e5c94-154">homepage</span></span>|<span data-ttu-id="e5c94-155">String</span><span class="sxs-lookup"><span data-stu-id="e5c94-155">String</span></span>|<span data-ttu-id="e5c94-156">A URL para a home page do aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="e5c94-156">The URL to the homepage of the associated application.</span></span>|
|<span data-ttu-id="e5c94-157">keyCredentials</span><span class="sxs-lookup"><span data-stu-id="e5c94-157">keyCredentials</span></span>|<span data-ttu-id="e5c94-158">microsoft.graph.keyCredential</span><span class="sxs-lookup"><span data-stu-id="e5c94-158">microsoft.graph.keyCredential</span></span>|<span data-ttu-id="e5c94-159">A coleção de credenciais de chave associado ao serviço principal.</span><span class="sxs-lookup"><span data-stu-id="e5c94-159">The collection of key credentials associated with the service principal.</span></span>                            <span data-ttu-id="e5c94-160">**Anotações**: não anulável.</span><span class="sxs-lookup"><span data-stu-id="e5c94-160">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="e5c94-161">logoutUrl</span><span class="sxs-lookup"><span data-stu-id="e5c94-161">logoutUrl</span></span>|<span data-ttu-id="e5c94-162">String</span><span class="sxs-lookup"><span data-stu-id="e5c94-162">String</span></span>| <span data-ttu-id="e5c94-163">Especifica a URL que será usada pelo serviço de autorização da Microsoft para logout um usuário usando o [canal de frente](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) ou protocolos de logout SAML.</span><span class="sxs-lookup"><span data-stu-id="e5c94-163">Specifies the URL that will be used by Microsoft's authorization service to logout an user using [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) or SAML logout protocols.</span></span> |
|<span data-ttu-id="e5c94-164">oauth2Permissions</span><span class="sxs-lookup"><span data-stu-id="e5c94-164">oauth2Permissions</span></span>|<span data-ttu-id="e5c94-165">microsoft.graph.oAuth2Permission</span><span class="sxs-lookup"><span data-stu-id="e5c94-165">microsoft.graph.oAuth2Permission</span></span>|<span data-ttu-id="e5c94-166">As permissões de OAuth 2.0 expostas pelo aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="e5c94-166">The OAuth 2.0 permissions exposed by the associated application.</span></span> <span data-ttu-id="e5c94-167">Para obter mais informações, consulte a definição da propriedade **oauth2Permissions** sobre a entidade de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e5c94-167">For more information see the **oauth2Permissions** property definition on the application entity.</span></span>                            <span data-ttu-id="e5c94-168">**Observações**: requer a versão 1.5 ou mais recente, não são nulas.</span><span class="sxs-lookup"><span data-stu-id="e5c94-168">**Notes**: Requires version 1.5 or newer, not nullable.</span></span>            |
|<span data-ttu-id="e5c94-169">passwordCredentials</span><span class="sxs-lookup"><span data-stu-id="e5c94-169">passwordCredentials</span></span>|<span data-ttu-id="e5c94-170">microsoft.graph.passwordCredential</span><span class="sxs-lookup"><span data-stu-id="e5c94-170">microsoft.graph.passwordCredential</span></span>|<span data-ttu-id="e5c94-171">A coleção de credenciais de senha associadas a entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="e5c94-171">The collection of password credentials associated with the service principal.</span></span>                            <span data-ttu-id="e5c94-172">**Anotações**: não anulável.</span><span class="sxs-lookup"><span data-stu-id="e5c94-172">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="e5c94-173">preferredTokenSigningKeyThumbprint</span><span class="sxs-lookup"><span data-stu-id="e5c94-173">preferredTokenSigningKeyThumbprint</span></span>|<span data-ttu-id="e5c94-174">String</span><span class="sxs-lookup"><span data-stu-id="e5c94-174">String</span></span>|<span data-ttu-id="e5c94-175">Reservado para uso interno apenas.</span><span class="sxs-lookup"><span data-stu-id="e5c94-175">Reserved for internal use only.</span></span> <span data-ttu-id="e5c94-176">Não gravar ou caso contrário, contam com esta propriedade.</span><span class="sxs-lookup"><span data-stu-id="e5c94-176">Do not write or otherwise rely on this property.</span></span> <span data-ttu-id="e5c94-177">Pode ser removido em futuras versões.</span><span class="sxs-lookup"><span data-stu-id="e5c94-177">May be removed in future versions.</span></span>                            <span data-ttu-id="e5c94-178">**Observações**: requer a versão 1.5 ou mais recente.</span><span class="sxs-lookup"><span data-stu-id="e5c94-178">**Notes**: Requires version 1.5 or newer.</span></span>            |
|<span data-ttu-id="e5c94-179">publisherName</span><span class="sxs-lookup"><span data-stu-id="e5c94-179">publisherName</span></span>|<span data-ttu-id="e5c94-180">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e5c94-180">String</span></span>|<span data-ttu-id="e5c94-181">O nome de exibição do inquilino no qual o aplicativo associado for especificado.</span><span class="sxs-lookup"><span data-stu-id="e5c94-181">The display name of the tenant in which the associated application is specified.</span></span>|
|<span data-ttu-id="e5c94-182">replyUrls</span><span class="sxs-lookup"><span data-stu-id="e5c94-182">replyUrls</span></span>|<span data-ttu-id="e5c94-183">String</span><span class="sxs-lookup"><span data-stu-id="e5c94-183">String</span></span>|<span data-ttu-id="e5c94-184">As URLs que os tokens do usuário são enviados para entrada com o aplicativo associado ou o redirecionamento códigos de autorização de URIs que OAuth 2.0 e tokens de acesso são enviados para o aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="e5c94-184">The URLs that user tokens are sent to for sign in with the associated application, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to for the associated application.</span></span>                            <span data-ttu-id="e5c94-185">**Anotações**: não anulável.</span><span class="sxs-lookup"><span data-stu-id="e5c94-185">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="e5c94-186">samlMetadataUrl</span><span class="sxs-lookup"><span data-stu-id="e5c94-186">samlMetadataUrl</span></span>|<span data-ttu-id="e5c94-187">String</span><span class="sxs-lookup"><span data-stu-id="e5c94-187">String</span></span>|            |
|<span data-ttu-id="e5c94-188">servicePrincipalNames</span><span class="sxs-lookup"><span data-stu-id="e5c94-188">servicePrincipalNames</span></span>|<span data-ttu-id="e5c94-189">String</span><span class="sxs-lookup"><span data-stu-id="e5c94-189">String</span></span>|<span data-ttu-id="e5c94-190">Os URIs que identificam o aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="e5c94-190">The URIs that identify the associated application.</span></span> <span data-ttu-id="e5c94-191">Para mais informações, consulte [objetos de aplicativo e objetos de entidade de serviço](https://msdn.microsoft.com/library/azure/dn132633.aspx).</span><span class="sxs-lookup"><span data-stu-id="e5c94-191">For more information see, [Application Objects and Service Principal Objects](https://msdn.microsoft.com/library/azure/dn132633.aspx).</span></span>                            <span data-ttu-id="e5c94-192">**Observações**: não são nulas, o operador **any** é necessário para expressões de filtro propriedades de valores múltiplos; Para obter mais informações, consulte [suporte para consultas, filtros e opções de paginação](https://msdn.microsoft.com/library/azure/dn727074.aspx).</span><span class="sxs-lookup"><span data-stu-id="e5c94-192">**Notes**: not nullable, the **any** operator is required for filter expressions on multi-valued properties; for more information, see [Supported Queries, Filters, and Paging Options](https://msdn.microsoft.com/library/azure/dn727074.aspx).</span></span>            |
|<span data-ttu-id="e5c94-193">marcações</span><span class="sxs-lookup"><span data-stu-id="e5c94-193">tags</span></span>|<span data-ttu-id="e5c94-194">String</span><span class="sxs-lookup"><span data-stu-id="e5c94-194">String</span></span>|                                        <span data-ttu-id="e5c94-195">**Anotações**: não anulável.</span><span class="sxs-lookup"><span data-stu-id="e5c94-195">**Notes**: not nullable.</span></span>            |

## <a name="response"></a><span data-ttu-id="e5c94-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5c94-196">Response</span></span>

<span data-ttu-id="e5c94-197">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto atualizado [servicePrincipal](../resources/serviceprincipal.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e5c94-197">If successful, this method returns a `200 OK` response code and updated [servicePrincipal](../resources/serviceprincipal.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e5c94-198">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e5c94-198">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e5c94-199">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e5c94-199">Request</span></span>
<span data-ttu-id="e5c94-200">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e5c94-200">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_serviceprincipal"
}-->
```http
PATCH https://graph.microsoft.com/beta/servicePrincipals/{id}
Content-type: application/json
Content-length: 391

{
  "accountEnabled": true,
  "addIns": [
    {
      "id": "id-value",
      "type": "type-value",
      "properties": [
        {
          "key": "key-value",
          "value": "value-value"
        }
      ]
    }
  ],
  "appDisplayName": "appDisplayName-value",
  "appId": "appId-value",
  "appOwnerOrganizationId": "appOwnerOrganizationId-value",
  "appRoleAssignmentRequired": true
}
```
##### <a name="response"></a><span data-ttu-id="e5c94-201">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5c94-201">Response</span></span>
<span data-ttu-id="e5c94-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e5c94-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 391

{
  "accountEnabled": true,
  "addIns": [
    {
      "id": "id-value",
      "type": "type-value",
      "properties": [
        {
          "key": "key-value",
          "value": "value-value"
        }
      ]
    }
  ],
  "appDisplayName": "appDisplayName-value",
  "appId": "appId-value",
  "appOwnerOrganizationId": "appOwnerOrganizationId-value",
  "appRoleAssignmentRequired": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update serviceprincipal",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/serviceprincipal-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
