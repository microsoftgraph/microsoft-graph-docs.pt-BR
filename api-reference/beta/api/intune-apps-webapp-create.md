---
title: Criar webApp
description: Cria um novo objeto webApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 425933e759e0c30483c70d7ff29182337266d476
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42444865"
---
# <a name="create-webapp"></a><span data-ttu-id="1d4cd-103">Criar webApp</span><span class="sxs-lookup"><span data-stu-id="1d4cd-103">Create webApp</span></span>

<span data-ttu-id="1d4cd-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1d4cd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1d4cd-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1d4cd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1d4cd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1d4cd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d4cd-107">Cria um novo objeto [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="1d4cd-107">Create a new [webApp](../resources/intune-apps-webapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1d4cd-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1d4cd-108">Prerequisites</span></span>
<span data-ttu-id="1d4cd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d4cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d4cd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1d4cd-111">Permission type</span></span>|<span data-ttu-id="1d4cd-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1d4cd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1d4cd-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1d4cd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1d4cd-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d4cd-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1d4cd-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1d4cd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1d4cd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1d4cd-116">Not supported.</span></span>|
|<span data-ttu-id="1d4cd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1d4cd-117">Application</span></span>|<span data-ttu-id="1d4cd-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d4cd-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1d4cd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1d4cd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="1d4cd-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1d4cd-120">Request headers</span></span>
|<span data-ttu-id="1d4cd-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1d4cd-121">Header</span></span>|<span data-ttu-id="1d4cd-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1d4cd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1d4cd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1d4cd-123">Authorization</span></span>|<span data-ttu-id="1d4cd-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1d4cd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1d4cd-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1d4cd-125">Accept</span></span>|<span data-ttu-id="1d4cd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1d4cd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d4cd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1d4cd-127">Request body</span></span>
<span data-ttu-id="1d4cd-128">No corpo da solicitação, forneça uma representação JSON do objeto webApp.</span><span class="sxs-lookup"><span data-stu-id="1d4cd-128">In the request body, supply a JSON representation for the webApp object.</span></span>

<span data-ttu-id="1d4cd-129">A tabela a seguir mostra as propriedades obrigatórias ao criar o webApp.</span><span class="sxs-lookup"><span data-stu-id="1d4cd-129">The following table shows the properties that are required when you create the webApp.</span></span>

|<span data-ttu-id="1d4cd-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1d4cd-130">Property</span></span>|<span data-ttu-id="1d4cd-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1d4cd-131">Type</span></span>|<span data-ttu-id="1d4cd-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d4cd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d4cd-133">id</span><span class="sxs-lookup"><span data-stu-id="1d4cd-133">id</span></span>|<span data-ttu-id="1d4cd-134">String</span><span class="sxs-lookup"><span data-stu-id="1d4cd-134">String</span></span>|<span data-ttu-id="1d4cd-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="1d4cd-135">Key of the entity.</span></span> <span data-ttu-id="1d4cd-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1d4cd-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1d4cd-137">displayName</span><span class="sxs-lookup"><span data-stu-id="1d4cd-137">displayName</span></span>|<span data-ttu-id="1d4cd-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1d4cd-138">String</span></span>|<span data-ttu-id="1d4cd-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="1d4cd-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="1d4cd-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1d4cd-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1d4cd-141">description</span><span class="sxs-lookup"><span data-stu-id="1d4cd-141">description</span></span>|<span data-ttu-id="1d4cd-142">String</span><span class="sxs-lookup"><span data-stu-id="1d4cd-142">String</span></span>|<span data-ttu-id="1d4cd-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1d4cd-143">The description of the app.</span></span> <span data-ttu-id="1d4cd-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1d4cd-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1d4cd-145">publicador</span><span class="sxs-lookup"><span data-stu-id="1d4cd-145">publisher</span></span>|<span data-ttu-id="1d4cd-146">String</span><span class="sxs-lookup"><span data-stu-id="1d4cd-146">String</span></span>|<span data-ttu-id="1d4cd-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1d4cd-147">The publisher of the app.</span></span> <span data-ttu-id="1d4cd-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1d4cd-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1d4cd-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="1d4cd-149">largeIcon</span></span>|[<span data-ttu-id="1d4cd-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="1d4cd-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="1d4cd-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="1d4cd-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="1d4cd-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1d4cd-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1d4cd-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1d4cd-153">createdDateTime</span></span>|<span data-ttu-id="1d4cd-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d4cd-154">DateTimeOffset</span></span>|<span data-ttu-id="1d4cd-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1d4cd-155">The date and time the app was created.</span></span> <span data-ttu-id="1d4cd-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1d4cd-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1d4cd-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1d4cd-157">lastModifiedDateTime</span></span>|<span data-ttu-id="1d4cd-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d4cd-158">DateTimeOffset</span></span>|<span data-ttu-id="1d4cd-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="1d4cd-159">The date and time the app was last modified.</span></span> <span data-ttu-id="1d4cd-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1d4cd-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1d4cd-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="1d4cd-161">isFeatured</span></span>|<span data-ttu-id="1d4cd-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d4cd-162">Boolean</span></span>|<span data-ttu-id="1d4cd-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1d4cd-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1d4cd-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="1d4cd-164">privacyInformationUrl</span></span>|<span data-ttu-id="1d4cd-165">String</span><span class="sxs-lookup"><span data-stu-id="1d4cd-165">String</span></span>|<span data-ttu-id="1d4cd-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="1d4cd-166">The privacy statement Url.</span></span> <span data-ttu-id="1d4cd-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1d4cd-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1d4cd-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="1d4cd-168">informationUrl</span></span>|<span data-ttu-id="1d4cd-169">String</span><span class="sxs-lookup"><span data-stu-id="1d4cd-169">String</span></span>|<span data-ttu-id="1d4cd-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="1d4cd-170">The more information Url.</span></span> <span data-ttu-id="1d4cd-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1d4cd-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1d4cd-172">owner</span><span class="sxs-lookup"><span data-stu-id="1d4cd-172">owner</span></span>|<span data-ttu-id="1d4cd-173">String</span><span class="sxs-lookup"><span data-stu-id="1d4cd-173">String</span></span>|<span data-ttu-id="1d4cd-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="1d4cd-174">The owner of the app.</span></span> <span data-ttu-id="1d4cd-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1d4cd-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1d4cd-176">developer</span><span class="sxs-lookup"><span data-stu-id="1d4cd-176">developer</span></span>|<span data-ttu-id="1d4cd-177">String</span><span class="sxs-lookup"><span data-stu-id="1d4cd-177">String</span></span>|<span data-ttu-id="1d4cd-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1d4cd-178">The developer of the app.</span></span> <span data-ttu-id="1d4cd-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1d4cd-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1d4cd-180">notes</span><span class="sxs-lookup"><span data-stu-id="1d4cd-180">notes</span></span>|<span data-ttu-id="1d4cd-181">String</span><span class="sxs-lookup"><span data-stu-id="1d4cd-181">String</span></span>|<span data-ttu-id="1d4cd-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1d4cd-182">Notes for the app.</span></span> <span data-ttu-id="1d4cd-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1d4cd-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1d4cd-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="1d4cd-184">uploadState</span></span>|<span data-ttu-id="1d4cd-185">Int32</span><span class="sxs-lookup"><span data-stu-id="1d4cd-185">Int32</span></span>|<span data-ttu-id="1d4cd-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="1d4cd-186">The upload state.</span></span> <span data-ttu-id="1d4cd-187">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1d4cd-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1d4cd-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="1d4cd-188">publishingState</span></span>|[<span data-ttu-id="1d4cd-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="1d4cd-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="1d4cd-190">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1d4cd-190">The publishing state for the app.</span></span> <span data-ttu-id="1d4cd-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="1d4cd-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="1d4cd-192">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1d4cd-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="1d4cd-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="1d4cd-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="1d4cd-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="1d4cd-194">isAssigned</span></span>|<span data-ttu-id="1d4cd-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d4cd-195">Boolean</span></span>|<span data-ttu-id="1d4cd-196">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="1d4cd-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="1d4cd-197">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1d4cd-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1d4cd-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1d4cd-198">roleScopeTagIds</span></span>|<span data-ttu-id="1d4cd-199">String collection</span><span class="sxs-lookup"><span data-stu-id="1d4cd-199">String collection</span></span>|<span data-ttu-id="1d4cd-200">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="1d4cd-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="1d4cd-201">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1d4cd-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1d4cd-202">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="1d4cd-202">dependentAppCount</span></span>|<span data-ttu-id="1d4cd-203">Int32</span><span class="sxs-lookup"><span data-stu-id="1d4cd-203">Int32</span></span>|<span data-ttu-id="1d4cd-204">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="1d4cd-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="1d4cd-205">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1d4cd-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1d4cd-206">appUrl</span><span class="sxs-lookup"><span data-stu-id="1d4cd-206">appUrl</span></span>|<span data-ttu-id="1d4cd-207">String</span><span class="sxs-lookup"><span data-stu-id="1d4cd-207">String</span></span>|<span data-ttu-id="1d4cd-208">A URL do aplicativo Web.</span><span class="sxs-lookup"><span data-stu-id="1d4cd-208">The web app URL.</span></span>|
|<span data-ttu-id="1d4cd-209">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="1d4cd-209">useManagedBrowser</span></span>|<span data-ttu-id="1d4cd-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d4cd-210">Boolean</span></span>|<span data-ttu-id="1d4cd-211">Se o navegador gerenciado deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="1d4cd-211">Whether or not to use managed browser.</span></span> <span data-ttu-id="1d4cd-212">Essa propriedade só é aplicável ao Android e ao IOS.</span><span class="sxs-lookup"><span data-stu-id="1d4cd-212">This property is only applicable for Android and IOS.</span></span>|



## <a name="response"></a><span data-ttu-id="1d4cd-213">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d4cd-213">Response</span></span>
<span data-ttu-id="1d4cd-214">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [webApp](../resources/intune-apps-webapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1d4cd-214">If successful, this method returns a `201 Created` response code and a [webApp](../resources/intune-apps-webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d4cd-215">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1d4cd-215">Example</span></span>

### <a name="request"></a><span data-ttu-id="1d4cd-216">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1d4cd-216">Request</span></span>
<span data-ttu-id="1d4cd-217">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1d4cd-217">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 779

{
  "@odata.type": "#microsoft.graph.webApp",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "dependentAppCount": 1,
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```

### <a name="response"></a><span data-ttu-id="1d4cd-218">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d4cd-218">Response</span></span>
<span data-ttu-id="1d4cd-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1d4cd-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 951

{
  "@odata.type": "#microsoft.graph.webApp",
  "id": "4bdc5d30-5d30-4bdc-305d-dc4b305ddc4b",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "dependentAppCount": 1,
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```





