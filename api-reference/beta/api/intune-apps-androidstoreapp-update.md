---
title: Atualizar androidStoreApp
description: Atualiza as propriedades de um objeto androidStoreApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b7acff22e5873729a0195c5c57bb8852ded0977d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42445789"
---
# <a name="update-androidstoreapp"></a><span data-ttu-id="42719-103">Atualizar androidStoreApp</span><span class="sxs-lookup"><span data-stu-id="42719-103">Update androidStoreApp</span></span>

<span data-ttu-id="42719-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="42719-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="42719-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="42719-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42719-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="42719-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42719-107">Atualiza as propriedades de um objeto [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="42719-107">Update the properties of a [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="42719-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="42719-108">Prerequisites</span></span>
<span data-ttu-id="42719-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42719-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42719-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="42719-111">Permission type</span></span>|<span data-ttu-id="42719-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="42719-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42719-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="42719-113">Delegated (work or school account)</span></span>|<span data-ttu-id="42719-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42719-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="42719-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="42719-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42719-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42719-116">Not supported.</span></span>|
|<span data-ttu-id="42719-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="42719-117">Application</span></span>|<span data-ttu-id="42719-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42719-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="42719-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="42719-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="42719-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="42719-120">Request headers</span></span>
|<span data-ttu-id="42719-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="42719-121">Header</span></span>|<span data-ttu-id="42719-122">Valor</span><span class="sxs-lookup"><span data-stu-id="42719-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="42719-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="42719-123">Authorization</span></span>|<span data-ttu-id="42719-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="42719-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="42719-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="42719-125">Accept</span></span>|<span data-ttu-id="42719-126">application/json</span><span class="sxs-lookup"><span data-stu-id="42719-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="42719-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="42719-127">Request body</span></span>
<span data-ttu-id="42719-128">No corpo da solicitação, forneça uma representação JSON do objeto [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="42719-128">In the request body, supply a JSON representation for the [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

<span data-ttu-id="42719-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="42719-129">The following table shows the properties that are required when you create the [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span></span>

|<span data-ttu-id="42719-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="42719-130">Property</span></span>|<span data-ttu-id="42719-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="42719-131">Type</span></span>|<span data-ttu-id="42719-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="42719-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42719-133">id</span><span class="sxs-lookup"><span data-stu-id="42719-133">id</span></span>|<span data-ttu-id="42719-134">String</span><span class="sxs-lookup"><span data-stu-id="42719-134">String</span></span>|<span data-ttu-id="42719-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="42719-135">Key of the entity.</span></span> <span data-ttu-id="42719-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="42719-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="42719-137">displayName</span><span class="sxs-lookup"><span data-stu-id="42719-137">displayName</span></span>|<span data-ttu-id="42719-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="42719-138">String</span></span>|<span data-ttu-id="42719-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="42719-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="42719-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="42719-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="42719-141">description</span><span class="sxs-lookup"><span data-stu-id="42719-141">description</span></span>|<span data-ttu-id="42719-142">String</span><span class="sxs-lookup"><span data-stu-id="42719-142">String</span></span>|<span data-ttu-id="42719-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="42719-143">The description of the app.</span></span> <span data-ttu-id="42719-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="42719-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="42719-145">publicador</span><span class="sxs-lookup"><span data-stu-id="42719-145">publisher</span></span>|<span data-ttu-id="42719-146">String</span><span class="sxs-lookup"><span data-stu-id="42719-146">String</span></span>|<span data-ttu-id="42719-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="42719-147">The publisher of the app.</span></span> <span data-ttu-id="42719-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="42719-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="42719-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="42719-149">largeIcon</span></span>|[<span data-ttu-id="42719-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="42719-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="42719-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="42719-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="42719-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="42719-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="42719-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="42719-153">createdDateTime</span></span>|<span data-ttu-id="42719-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42719-154">DateTimeOffset</span></span>|<span data-ttu-id="42719-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="42719-155">The date and time the app was created.</span></span> <span data-ttu-id="42719-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="42719-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="42719-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="42719-157">lastModifiedDateTime</span></span>|<span data-ttu-id="42719-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42719-158">DateTimeOffset</span></span>|<span data-ttu-id="42719-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="42719-159">The date and time the app was last modified.</span></span> <span data-ttu-id="42719-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="42719-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="42719-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="42719-161">isFeatured</span></span>|<span data-ttu-id="42719-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="42719-162">Boolean</span></span>|<span data-ttu-id="42719-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="42719-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="42719-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="42719-164">privacyInformationUrl</span></span>|<span data-ttu-id="42719-165">String</span><span class="sxs-lookup"><span data-stu-id="42719-165">String</span></span>|<span data-ttu-id="42719-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="42719-166">The privacy statement Url.</span></span> <span data-ttu-id="42719-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="42719-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="42719-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="42719-168">informationUrl</span></span>|<span data-ttu-id="42719-169">String</span><span class="sxs-lookup"><span data-stu-id="42719-169">String</span></span>|<span data-ttu-id="42719-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="42719-170">The more information Url.</span></span> <span data-ttu-id="42719-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="42719-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="42719-172">owner</span><span class="sxs-lookup"><span data-stu-id="42719-172">owner</span></span>|<span data-ttu-id="42719-173">String</span><span class="sxs-lookup"><span data-stu-id="42719-173">String</span></span>|<span data-ttu-id="42719-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="42719-174">The owner of the app.</span></span> <span data-ttu-id="42719-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="42719-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="42719-176">developer</span><span class="sxs-lookup"><span data-stu-id="42719-176">developer</span></span>|<span data-ttu-id="42719-177">String</span><span class="sxs-lookup"><span data-stu-id="42719-177">String</span></span>|<span data-ttu-id="42719-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="42719-178">The developer of the app.</span></span> <span data-ttu-id="42719-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="42719-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="42719-180">notes</span><span class="sxs-lookup"><span data-stu-id="42719-180">notes</span></span>|<span data-ttu-id="42719-181">String</span><span class="sxs-lookup"><span data-stu-id="42719-181">String</span></span>|<span data-ttu-id="42719-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="42719-182">Notes for the app.</span></span> <span data-ttu-id="42719-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="42719-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="42719-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="42719-184">uploadState</span></span>|<span data-ttu-id="42719-185">Int32</span><span class="sxs-lookup"><span data-stu-id="42719-185">Int32</span></span>|<span data-ttu-id="42719-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="42719-186">The upload state.</span></span> <span data-ttu-id="42719-187">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="42719-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="42719-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="42719-188">publishingState</span></span>|[<span data-ttu-id="42719-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="42719-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="42719-190">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="42719-190">The publishing state for the app.</span></span> <span data-ttu-id="42719-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="42719-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="42719-192">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="42719-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="42719-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="42719-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="42719-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="42719-194">isAssigned</span></span>|<span data-ttu-id="42719-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="42719-195">Boolean</span></span>|<span data-ttu-id="42719-196">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="42719-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="42719-197">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="42719-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="42719-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="42719-198">roleScopeTagIds</span></span>|<span data-ttu-id="42719-199">String collection</span><span class="sxs-lookup"><span data-stu-id="42719-199">String collection</span></span>|<span data-ttu-id="42719-200">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="42719-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="42719-201">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="42719-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="42719-202">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="42719-202">dependentAppCount</span></span>|<span data-ttu-id="42719-203">Int32</span><span class="sxs-lookup"><span data-stu-id="42719-203">Int32</span></span>|<span data-ttu-id="42719-204">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="42719-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="42719-205">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="42719-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="42719-206">packageId</span><span class="sxs-lookup"><span data-stu-id="42719-206">packageId</span></span>|<span data-ttu-id="42719-207">String</span><span class="sxs-lookup"><span data-stu-id="42719-207">String</span></span>|<span data-ttu-id="42719-208">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="42719-208">The package identifier.</span></span>|
|<span data-ttu-id="42719-209">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="42719-209">appIdentifier</span></span>|<span data-ttu-id="42719-210">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="42719-210">String</span></span>|<span data-ttu-id="42719-211">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="42719-211">The Identity Name.</span></span>|
|<span data-ttu-id="42719-212">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="42719-212">appStoreUrl</span></span>|<span data-ttu-id="42719-213">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="42719-213">String</span></span>|<span data-ttu-id="42719-214">A URL da loja de aplicativos Android.</span><span class="sxs-lookup"><span data-stu-id="42719-214">The Android app store URL.</span></span>|
|<span data-ttu-id="42719-215">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="42719-215">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="42719-216">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="42719-216">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="42719-217">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="42719-217">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="42719-218">Resposta</span><span class="sxs-lookup"><span data-stu-id="42719-218">Response</span></span>
<span data-ttu-id="42719-219">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [androidStoreApp](../resources/intune-apps-androidstoreapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="42719-219">If successful, this method returns a `200 OK` response code and an updated [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42719-220">Exemplo</span><span class="sxs-lookup"><span data-stu-id="42719-220">Example</span></span>

### <a name="request"></a><span data-ttu-id="42719-221">Solicitação</span><span class="sxs-lookup"><span data-stu-id="42719-221">Request</span></span>
<span data-ttu-id="42719-222">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="42719-222">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1230

{
  "@odata.type": "#microsoft.graph.androidStoreApp",
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
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="42719-223">Resposta</span><span class="sxs-lookup"><span data-stu-id="42719-223">Response</span></span>
<span data-ttu-id="42719-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="42719-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1402

{
  "@odata.type": "#microsoft.graph.androidStoreApp",
  "id": "1f2b7654-7654-1f2b-5476-2b1f54762b1f",
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
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  }
}
```





