---
title: Atualizar serviceprincipal
description: Atualizar as propriedades do objeto serviceprincipal.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: ad469a68a2dabd31d4f6c1b7ea52dd188f9e10b5
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055775"
---
# <a name="update-serviceprincipal"></a><span data-ttu-id="e459d-103">Atualizar servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="e459d-103">Update servicePrincipal</span></span>

<span data-ttu-id="e459d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e459d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e459d-105">Atualizar as propriedades do objeto [servicePrincipal](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="e459d-105">Update the properties of [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="e459d-106">Não há suporte para o uso do PATCH para definir [**passwordCredential**](../resources/passwordcredential.md).</span><span class="sxs-lookup"><span data-stu-id="e459d-106">Using PATCH to set [**passwordCredential**](../resources/passwordcredential.md) is not supported.</span></span> <span data-ttu-id="e459d-107">Use os métodos [addPassword](./serviceprincipal-addpassword.md) e [removePassword](./serviceprincipal-removepassword.md) para atualizá-la para uma entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="e459d-107">Use the [addPassword](./serviceprincipal-addpassword.md) and [removePassword](./serviceprincipal-removepassword.md) methods to update the password for a servicePrincipal.</span></span>

## <a name="permissions"></a><span data-ttu-id="e459d-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="e459d-108">Permissions</span></span>
<span data-ttu-id="e459d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e459d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e459d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e459d-111">Permission type</span></span>      | <span data-ttu-id="e459d-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e459d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e459d-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e459d-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e459d-114">Application.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e459d-114">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e459d-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e459d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e459d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e459d-116">Not supported.</span></span>    |
|<span data-ttu-id="e459d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e459d-117">Application</span></span> | <span data-ttu-id="e459d-118">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e459d-118">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e459d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e459d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /servicePrincipals/{id}
```
## <a name="request-headers"></a><span data-ttu-id="e459d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e459d-120">Request headers</span></span>
| <span data-ttu-id="e459d-121">Nome</span><span class="sxs-lookup"><span data-stu-id="e459d-121">Name</span></span>       | <span data-ttu-id="e459d-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e459d-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="e459d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e459d-123">Authorization</span></span> | <span data-ttu-id="e459d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e459d-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e459d-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e459d-126">Content-Type</span></span> | <span data-ttu-id="e459d-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e459d-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e459d-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e459d-129">Request body</span></span>
<span data-ttu-id="e459d-p105">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="e459d-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e459d-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e459d-133">Property</span></span>     | <span data-ttu-id="e459d-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="e459d-134">Type</span></span> |<span data-ttu-id="e459d-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="e459d-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e459d-136">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="e459d-136">accountEnabled</span></span>|<span data-ttu-id="e459d-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="e459d-137">Boolean</span></span>| <span data-ttu-id="e459d-138">**True** se a entidade de serviço estiver habilitada; caso contrário, **false**.</span><span class="sxs-lookup"><span data-stu-id="e459d-138">**true** if the service principal account is enabled; otherwise, **false**.</span></span>|
|<span data-ttu-id="e459d-139">addIns</span><span class="sxs-lookup"><span data-stu-id="e459d-139">addIns</span></span>| [<span data-ttu-id="e459d-140">addIn</span><span class="sxs-lookup"><span data-stu-id="e459d-140">addIn</span></span>](../resources/addin.md) | <span data-ttu-id="e459d-141">Define o comportamento personalizado que um serviço de consumo pode usar para chamar um aplicativo em contextos específicos.</span><span class="sxs-lookup"><span data-stu-id="e459d-141">Defines custom behavior that a consuming service can use to call an app in specific contexts.</span></span> <span data-ttu-id="e459d-142">Por exemplo, aplicativos que podem renderizar fluxos de arquivo [podem definir a propriedade addIns](/onedrive/developer/file-handlers/?view=odsp-graph-online) para a funcionalidade "FileHandler".</span><span class="sxs-lookup"><span data-stu-id="e459d-142">For example, applications that can render file streams [may set the addIns property](/onedrive/developer/file-handlers/?view=odsp-graph-online) for its "FileHandler" functionality.</span></span> <span data-ttu-id="e459d-143">Isso permitirá que os serviços como o Microsoft 365 chamem o aplicativo no contexto de um documento no qual o usuário esteja trabalhando.</span><span class="sxs-lookup"><span data-stu-id="e459d-143">This will let services like Microsoft 365 call the application in the context of a document the user is working on.</span></span>|
|<span data-ttu-id="e459d-144">alternativeNames</span><span class="sxs-lookup"><span data-stu-id="e459d-144">alternativeNames</span></span>|<span data-ttu-id="e459d-145">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e459d-145">String collection</span></span>| <span data-ttu-id="e459d-146">Usado para recuperar entidades de serviço por assinatura, identificar grupo de recursos e IDs de recursos completos de [identidades gerenciadas](https://aka.ms/azuremanagedidentity).</span><span class="sxs-lookup"><span data-stu-id="e459d-146">Used to retrieve service principals by subscription, identify resource group and full resource ids for [managed identities](https://aka.ms/azuremanagedidentity).</span></span>|
|<span data-ttu-id="e459d-147">appRoleAssignmentRequired</span><span class="sxs-lookup"><span data-stu-id="e459d-147">appRoleAssignmentRequired</span></span>|<span data-ttu-id="e459d-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="e459d-148">Boolean</span></span>|<span data-ttu-id="e459d-149">Especifica se um **appRoleAssignment** de um usuário ou grupo é necessário antes que o Azure AD emita um token de usuário ou de acesso ao aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e459d-149">Specifies whether an **appRoleAssignment** to a user or group is required before Azure AD will issue a user or access token to the application.</span></span> <span data-ttu-id="e459d-150">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="e459d-150">Not nullable.</span></span> |
|<span data-ttu-id="e459d-151">appRoles</span><span class="sxs-lookup"><span data-stu-id="e459d-151">appRoles</span></span>|<span data-ttu-id="e459d-152">[appRole](../resources/approle.md) collection</span><span class="sxs-lookup"><span data-stu-id="e459d-152">[appRole](../resources/approle.md) collection</span></span>|<span data-ttu-id="e459d-153">As funções do aplicativo expostas pelo aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="e459d-153">The application roles exposed by the associated application.</span></span> <span data-ttu-id="e459d-154">Para obter mais informações, confira a definição da propriedade **appRoles** no recurso [aplicativo](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="e459d-154">For more information see the **appRoles** property definition on the [application](../resources/application.md) resource.</span></span> <span data-ttu-id="e459d-155">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="e459d-155">Not nullable.</span></span> |
|<span data-ttu-id="e459d-156">displayName</span><span class="sxs-lookup"><span data-stu-id="e459d-156">displayName</span></span>|<span data-ttu-id="e459d-157">String</span><span class="sxs-lookup"><span data-stu-id="e459d-157">String</span></span>|<span data-ttu-id="e459d-158">O nome de exibição da entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="e459d-158">The display name for the service principal.</span></span>|
|<span data-ttu-id="e459d-159">homepage</span><span class="sxs-lookup"><span data-stu-id="e459d-159">homepage</span></span>|<span data-ttu-id="e459d-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e459d-160">String</span></span>|<span data-ttu-id="e459d-161">Página inicial ou página de aterrissagem do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e459d-161">Home page or landing page of the application.</span></span>|
|<span data-ttu-id="e459d-162">keyCredentials</span><span class="sxs-lookup"><span data-stu-id="e459d-162">keyCredentials</span></span>|<span data-ttu-id="e459d-163">[keyCredential](../resources/keycredential.md) collection</span><span class="sxs-lookup"><span data-stu-id="e459d-163">[keyCredential](../resources/keycredential.md) collection</span></span>|<span data-ttu-id="e459d-p109">A coleta de principais credenciais associadas ao diretor de serviços. Não pode ser anulado.</span><span class="sxs-lookup"><span data-stu-id="e459d-p109">The collection of key credentials associated with the service principal. Not nullable.</span></span>            |
|<span data-ttu-id="e459d-166">logoutUrl</span><span class="sxs-lookup"><span data-stu-id="e459d-166">logoutUrl</span></span>|<span data-ttu-id="e459d-167">String</span><span class="sxs-lookup"><span data-stu-id="e459d-167">String</span></span>| <span data-ttu-id="e459d-168">Especifica a URL que será usada pela autorização do serviço da Microsoft para fazer logoff de um usuário usando protocolos de logoff [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) ou SAML.</span><span class="sxs-lookup"><span data-stu-id="e459d-168">Specifies the URL that will be used by Microsoft's authorization service to logout an user using [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) or SAML logout protocols.</span></span>|
|<span data-ttu-id="e459d-169">oauth2PermissionScopes</span><span class="sxs-lookup"><span data-stu-id="e459d-169">oauth2PermissionScopes</span></span>|<span data-ttu-id="e459d-170">coleção [permissionScope](../resources/permissionScope.md)</span><span class="sxs-lookup"><span data-stu-id="e459d-170">[permissionScope](../resources/permissionScope.md) collection</span></span>|<span data-ttu-id="e459d-171">As permissões do escopo OAuth 2.0 expostas pelo aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="e459d-171">The OAuth 2.0 permission scopes exposed by the associated application.</span></span> <span data-ttu-id="e459d-172">Para obter mais informações, confira a definição da propriedade **oauth2PermissionScopes** no recurso [aplicativo](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="e459d-172">For more information see the **oauth2PermissionScopes** property definition on the [application](../resources/application.md) resource.</span></span> <span data-ttu-id="e459d-173">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="e459d-173">Not nullable.</span></span>|
|<span data-ttu-id="e459d-174">preferredSingleSignOnMode</span><span class="sxs-lookup"><span data-stu-id="e459d-174">preferredSingleSignOnMode</span></span>|<span data-ttu-id="e459d-175">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e459d-175">string</span></span>|<span data-ttu-id="e459d-176">Especifica o modo de logon único configurado para este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e459d-176">Specifies the single sign-on mode configured for this application.</span></span> <span data-ttu-id="e459d-177">O Azure AD usa o modo de logon único preferido para iniciar o aplicativo do Microsoft 365 ou o Azure AD My Apps.</span><span class="sxs-lookup"><span data-stu-id="e459d-177">Azure AD uses the preferred single sign-on mode to launch the application from Microsoft 365 or the Azure AD My Apps.</span></span> <span data-ttu-id="e459d-178">Os valores com suporte são: `password`, `saml`, `external`, e `oidc`.</span><span class="sxs-lookup"><span data-stu-id="e459d-178">The supported values are `password`, `saml`, `external`, and `oidc`.</span></span>|
|<span data-ttu-id="e459d-179">replyUrls</span><span class="sxs-lookup"><span data-stu-id="e459d-179">replyUrls</span></span>|<span data-ttu-id="e459d-180">String collection</span><span class="sxs-lookup"><span data-stu-id="e459d-180">String collection</span></span>|<span data-ttu-id="e459d-p112">URLs para as quais os tokens de usuário são enviados para se conectar com a aplicação associada, ou as URIs redirecionadas para as quais os códigos de autorização OAuth 2.0 e os tokens de acesso são enviados para a aplicação associada. Não pode ser anulado.</span><span class="sxs-lookup"><span data-stu-id="e459d-p112">The URLs that user tokens are sent to for sign in with the associated application, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to for the associated application. Not nullable.</span></span> |
|<span data-ttu-id="e459d-183">servicePrincipalNames</span><span class="sxs-lookup"><span data-stu-id="e459d-183">servicePrincipalNames</span></span>|<span data-ttu-id="e459d-184">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e459d-184">String collection</span></span>|<span data-ttu-id="e459d-185">Contém a lista de **identificadoresUris**, copiados do [aplicativo](../resources/application.md) associado.</span><span class="sxs-lookup"><span data-stu-id="e459d-185">Contains the list of **identifiersUris**, copied over from the associated [application](../resources/application.md).</span></span> <span data-ttu-id="e459d-186">É possível adicionar valores adicionais aos aplicativos híbridos.</span><span class="sxs-lookup"><span data-stu-id="e459d-186">Additional values can be added to hybrid applications.</span></span> <span data-ttu-id="e459d-187">Esses valores podem ser usados ​​para identificar as permissões apresentadas por esse aplicativo no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e459d-187">These values can be used to identify the permissions exposed by this app within Azure AD.</span></span> <span data-ttu-id="e459d-188">Por exemplo,</span><span class="sxs-lookup"><span data-stu-id="e459d-188">For example,</span></span><ul><li><span data-ttu-id="e459d-189">Os aplicativos cliente solicitando permissões para este recurso podem usar esses URIs para especificar as permissões necessárias na propriedade **requiredResourceAccess** do manifesto do aplicativo, ou na lâmina "permissões de API" na experiência de registros de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="e459d-189">Client apps requesting permissions to this resource can use these URIs to specify needed permissions in the **requiredResourceAccess** property of their application manifest, or in the "API permissions" blade on the App registrations experience.</span></span></li><li><span data-ttu-id="e459d-190">Os aplicativos cliente podem especificar um URI de recurso com base nos valores dessa propriedade para adquirir um token de acesso, que é o URI retornado na declaração "aud".</span><span class="sxs-lookup"><span data-stu-id="e459d-190">Client apps can specify a resource URI which is based on the values of this property to acquire an access token, which is the URI returned in the “aud” claim.</span></span></li></ul><br><span data-ttu-id="e459d-p114">O operador é necessário para filtrar expressões nas propriedades multivalorizadas. Não pode ser anulado.</span><span class="sxs-lookup"><span data-stu-id="e459d-p114">The any operator is required for filter expressions on multi-valued properties. Not nullable.</span></span>|
|<span data-ttu-id="e459d-193">tags</span><span class="sxs-lookup"><span data-stu-id="e459d-193">tags</span></span>|<span data-ttu-id="e459d-194">Coleção String</span><span class="sxs-lookup"><span data-stu-id="e459d-194">String collection</span></span>| <span data-ttu-id="e459d-p115">Cadeias de caracteres personalizadas que podem ser usadas para categorizar e identificar o aplicativo. Não anulada.</span><span class="sxs-lookup"><span data-stu-id="e459d-p115">Custom strings that can be used to categorize and identify the application. Not nullable.</span></span> |
| <span data-ttu-id="e459d-197">tokenEncryptionKeyId</span><span class="sxs-lookup"><span data-stu-id="e459d-197">tokenEncryptionKeyId</span></span> |<span data-ttu-id="e459d-198">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e459d-198">String</span></span>|<span data-ttu-id="e459d-199">Especifica a keyId de uma chave pública da coleção keyCredentials.</span><span class="sxs-lookup"><span data-stu-id="e459d-199">Specifies the keyId of a public key from the keyCredentials collection.</span></span> <span data-ttu-id="e459d-200">Quando configurado, o Azure AD emite tokens para este aplicativo criptografado usando a chave especificada por essa propriedade.</span><span class="sxs-lookup"><span data-stu-id="e459d-200">When configured, Azure AD issues tokens for this application encrypted using the key specified by this property.</span></span> <span data-ttu-id="e459d-201">O código de aplicativo que recebe o token criptografado deve usar a chave privada correspondente para descriptografar o token a fim de que ele possa ser usado para o usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="e459d-201">The application code that receives the encrypted token must use the matching private key to decrypt the token before it can be used for the signed-in user.</span></span>|

## <a name="response"></a><span data-ttu-id="e459d-202">Resposta</span><span class="sxs-lookup"><span data-stu-id="e459d-202">Response</span></span>

<span data-ttu-id="e459d-203">Se bem-sucedido, este método retorna um código de resposta `204 No Content` e um objeto atualizado [servicePrincipal](../resources/serviceprincipal.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e459d-203">If successful, this method returns a `204 No Content` response code and updated [servicePrincipal](../resources/serviceprincipal.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e459d-204">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e459d-204">Example</span></span>
### <a name="request"></a><span data-ttu-id="e459d-205">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e459d-205">Request</span></span>
<span data-ttu-id="e459d-206">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e459d-206">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e459d-207">HTTP</span><span class="sxs-lookup"><span data-stu-id="e459d-207">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_serviceprincipal"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/servicePrincipals/{id}
Content-type: application/json
Content-length: 391

{
  "appRoleAssignmentRequired": true
}
```
# <a name="c"></a>[<span data-ttu-id="e459d-208">C#</span><span class="sxs-lookup"><span data-stu-id="e459d-208">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e459d-209">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e459d-209">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e459d-210">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e459d-210">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e459d-211">Java</span><span class="sxs-lookup"><span data-stu-id="e459d-211">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e459d-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="e459d-212">Response</span></span>
<span data-ttu-id="e459d-213">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e459d-213">Here is an example of the response.</span></span> <span data-ttu-id="e459d-214">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e459d-214">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal"
} -->
```http
HTTP/1.1 204 No Content
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
  ]
}
-->

