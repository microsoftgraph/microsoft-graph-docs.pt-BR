---
title: Atualizar androidStoreApp
description: Atualiza as propriedades de um objeto androidStoreApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d16efd41fb6bc207a5ab5face46dc90e019ee553
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30171348"
---
# <a name="update-androidstoreapp"></a><span data-ttu-id="8e188-103">Atualizar androidStoreApp</span><span class="sxs-lookup"><span data-stu-id="8e188-103">Update androidStoreApp</span></span>

> <span data-ttu-id="8e188-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8e188-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8e188-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8e188-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e188-106">Atualiza as propriedades de um objeto [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="8e188-106">Update the properties of a [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8e188-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8e188-107">Prerequisites</span></span>
<span data-ttu-id="8e188-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="8e188-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="8e188-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8e188-110">Permission type</span></span>|<span data-ttu-id="8e188-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8e188-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e188-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8e188-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8e188-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e188-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8e188-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8e188-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e188-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8e188-115">Not supported.</span></span>|
|<span data-ttu-id="8e188-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8e188-116">Application</span></span>|<span data-ttu-id="8e188-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8e188-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e188-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8e188-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="8e188-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8e188-119">Request headers</span></span>
|<span data-ttu-id="8e188-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8e188-120">Header</span></span>|<span data-ttu-id="8e188-121">Valor</span><span class="sxs-lookup"><span data-stu-id="8e188-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8e188-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8e188-122">Authorization</span></span>|<span data-ttu-id="8e188-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8e188-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8e188-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8e188-124">Accept</span></span>|<span data-ttu-id="8e188-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8e188-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e188-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8e188-126">Request body</span></span>
<span data-ttu-id="8e188-127">No corpo da solicitação, forneça uma representação JSON do objeto [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="8e188-127">In the request body, supply a JSON representation for the [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

<span data-ttu-id="8e188-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="8e188-128">The following table shows the properties that are required when you create the [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span></span>

|<span data-ttu-id="8e188-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8e188-129">Property</span></span>|<span data-ttu-id="8e188-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="8e188-130">Type</span></span>|<span data-ttu-id="8e188-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e188-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e188-132">id</span><span class="sxs-lookup"><span data-stu-id="8e188-132">id</span></span>|<span data-ttu-id="8e188-133">String</span><span class="sxs-lookup"><span data-stu-id="8e188-133">String</span></span>|<span data-ttu-id="8e188-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="8e188-134">Key of the entity.</span></span> <span data-ttu-id="8e188-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8e188-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8e188-136">displayName</span><span class="sxs-lookup"><span data-stu-id="8e188-136">displayName</span></span>|<span data-ttu-id="8e188-137">String</span><span class="sxs-lookup"><span data-stu-id="8e188-137">String</span></span>|<span data-ttu-id="8e188-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="8e188-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="8e188-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8e188-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8e188-140">description</span><span class="sxs-lookup"><span data-stu-id="8e188-140">description</span></span>|<span data-ttu-id="8e188-141">String</span><span class="sxs-lookup"><span data-stu-id="8e188-141">String</span></span>|<span data-ttu-id="8e188-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8e188-142">The description of the app.</span></span> <span data-ttu-id="8e188-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8e188-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8e188-144">publisher</span><span class="sxs-lookup"><span data-stu-id="8e188-144">publisher</span></span>|<span data-ttu-id="8e188-145">String</span><span class="sxs-lookup"><span data-stu-id="8e188-145">String</span></span>|<span data-ttu-id="8e188-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8e188-146">The publisher of the app.</span></span> <span data-ttu-id="8e188-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8e188-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8e188-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="8e188-148">largeIcon</span></span>|[<span data-ttu-id="8e188-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="8e188-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="8e188-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="8e188-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="8e188-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8e188-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8e188-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8e188-152">createdDateTime</span></span>|<span data-ttu-id="8e188-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e188-153">DateTimeOffset</span></span>|<span data-ttu-id="8e188-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8e188-154">The date and time the app was created.</span></span> <span data-ttu-id="8e188-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8e188-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8e188-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8e188-156">lastModifiedDateTime</span></span>|<span data-ttu-id="8e188-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e188-157">DateTimeOffset</span></span>|<span data-ttu-id="8e188-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="8e188-158">The date and time the app was last modified.</span></span> <span data-ttu-id="8e188-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8e188-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8e188-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="8e188-160">isFeatured</span></span>|<span data-ttu-id="8e188-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="8e188-161">Boolean</span></span>|<span data-ttu-id="8e188-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8e188-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8e188-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="8e188-163">privacyInformationUrl</span></span>|<span data-ttu-id="8e188-164">String</span><span class="sxs-lookup"><span data-stu-id="8e188-164">String</span></span>|<span data-ttu-id="8e188-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="8e188-165">The privacy statement Url.</span></span> <span data-ttu-id="8e188-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8e188-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8e188-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="8e188-167">informationUrl</span></span>|<span data-ttu-id="8e188-168">String</span><span class="sxs-lookup"><span data-stu-id="8e188-168">String</span></span>|<span data-ttu-id="8e188-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="8e188-169">The more information Url.</span></span> <span data-ttu-id="8e188-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8e188-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8e188-171">owner</span><span class="sxs-lookup"><span data-stu-id="8e188-171">owner</span></span>|<span data-ttu-id="8e188-172">String</span><span class="sxs-lookup"><span data-stu-id="8e188-172">String</span></span>|<span data-ttu-id="8e188-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="8e188-173">The owner of the app.</span></span> <span data-ttu-id="8e188-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8e188-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8e188-175">developer</span><span class="sxs-lookup"><span data-stu-id="8e188-175">developer</span></span>|<span data-ttu-id="8e188-176">String</span><span class="sxs-lookup"><span data-stu-id="8e188-176">String</span></span>|<span data-ttu-id="8e188-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8e188-177">The developer of the app.</span></span> <span data-ttu-id="8e188-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8e188-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8e188-179">Observações</span><span class="sxs-lookup"><span data-stu-id="8e188-179">notes</span></span>|<span data-ttu-id="8e188-180">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8e188-180">String</span></span>|<span data-ttu-id="8e188-181">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8e188-181">Notes for the app.</span></span> <span data-ttu-id="8e188-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8e188-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8e188-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="8e188-183">uploadState</span></span>|<span data-ttu-id="8e188-184">Int32</span><span class="sxs-lookup"><span data-stu-id="8e188-184">Int32</span></span>|<span data-ttu-id="8e188-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="8e188-185">The upload state.</span></span> <span data-ttu-id="8e188-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8e188-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8e188-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="8e188-187">publishingState</span></span>|[<span data-ttu-id="8e188-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="8e188-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="8e188-189">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8e188-189">The publishing state for the app.</span></span> <span data-ttu-id="8e188-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="8e188-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="8e188-191">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8e188-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="8e188-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="8e188-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="8e188-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="8e188-193">isAssigned</span></span>|<span data-ttu-id="8e188-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="8e188-194">Boolean</span></span>|<span data-ttu-id="8e188-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="8e188-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="8e188-196">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8e188-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8e188-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8e188-197">roleScopeTagIds</span></span>|<span data-ttu-id="8e188-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8e188-198">String collection</span></span>|<span data-ttu-id="8e188-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="8e188-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="8e188-200">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8e188-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8e188-201">packageId</span><span class="sxs-lookup"><span data-stu-id="8e188-201">packageId</span></span>|<span data-ttu-id="8e188-202">String</span><span class="sxs-lookup"><span data-stu-id="8e188-202">String</span></span>|<span data-ttu-id="8e188-203">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="8e188-203">The package identifier.</span></span>|
|<span data-ttu-id="8e188-204">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="8e188-204">appIdentifier</span></span>|<span data-ttu-id="8e188-205">String</span><span class="sxs-lookup"><span data-stu-id="8e188-205">String</span></span>|<span data-ttu-id="8e188-206">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="8e188-206">The Identity Name.</span></span>|
|<span data-ttu-id="8e188-207">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="8e188-207">appStoreUrl</span></span>|<span data-ttu-id="8e188-208">String</span><span class="sxs-lookup"><span data-stu-id="8e188-208">String</span></span>|<span data-ttu-id="8e188-209">A URL da loja de aplicativos Android.</span><span class="sxs-lookup"><span data-stu-id="8e188-209">The Android app store URL.</span></span>|
|<span data-ttu-id="8e188-210">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="8e188-210">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="8e188-211">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="8e188-211">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="8e188-212">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="8e188-212">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="8e188-213">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e188-213">Response</span></span>
<span data-ttu-id="8e188-214">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [androidStoreApp](../resources/intune-apps-androidstoreapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8e188-214">If successful, this method returns a `200 OK` response code and an updated [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e188-215">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8e188-215">Example</span></span>

### <a name="request"></a><span data-ttu-id="8e188-216">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8e188-216">Request</span></span>
<span data-ttu-id="8e188-217">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8e188-217">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1203

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

### <a name="response"></a><span data-ttu-id="8e188-218">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e188-218">Response</span></span>
<span data-ttu-id="8e188-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8e188-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1375

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




