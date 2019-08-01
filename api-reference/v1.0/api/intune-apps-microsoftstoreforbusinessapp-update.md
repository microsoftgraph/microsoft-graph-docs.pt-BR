---
title: Atualizar microsoftStoreForBusinessApp
description: Atualiza as propriedades de um objeto microsoftStoreForBusinessApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 053721e2bc58258e4f6d4d28478ce1bbd736e520
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36002108"
---
# <a name="update-microsoftstoreforbusinessapp"></a><span data-ttu-id="4c9d3-103">Atualizar microsoftStoreForBusinessApp</span><span class="sxs-lookup"><span data-stu-id="4c9d3-103">Update microsoftStoreForBusinessApp</span></span>

> <span data-ttu-id="4c9d3-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4c9d3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c9d3-105">Atualiza as propriedades de um objeto [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="4c9d3-105">Update the properties of a [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4c9d3-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4c9d3-106">Prerequisites</span></span>
<span data-ttu-id="4c9d3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c9d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c9d3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4c9d3-109">Permission type</span></span>|<span data-ttu-id="4c9d3-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4c9d3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4c9d3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4c9d3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4c9d3-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c9d3-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4c9d3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4c9d3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4c9d3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4c9d3-114">Not supported.</span></span>|
|<span data-ttu-id="4c9d3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4c9d3-115">Application</span></span>|<span data-ttu-id="4c9d3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4c9d3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c9d3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4c9d3-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="4c9d3-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4c9d3-118">Request headers</span></span>
|<span data-ttu-id="4c9d3-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4c9d3-119">Header</span></span>|<span data-ttu-id="4c9d3-120">Valor</span><span class="sxs-lookup"><span data-stu-id="4c9d3-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4c9d3-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4c9d3-121">Authorization</span></span>|<span data-ttu-id="4c9d3-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4c9d3-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4c9d3-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4c9d3-123">Accept</span></span>|<span data-ttu-id="4c9d3-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4c9d3-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c9d3-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4c9d3-125">Request body</span></span>
<span data-ttu-id="4c9d3-126">No corpo da solicitação, forneça uma representação JSON do objeto [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="4c9d3-126">In the request body, supply a JSON representation for the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

<span data-ttu-id="4c9d3-127">A tabela a seguir mostra as propriedades obrigatórias ao criar [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="4c9d3-127">The following table shows the properties that are required when you create the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span></span>

|<span data-ttu-id="4c9d3-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4c9d3-128">Property</span></span>|<span data-ttu-id="4c9d3-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="4c9d3-129">Type</span></span>|<span data-ttu-id="4c9d3-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c9d3-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c9d3-131">id</span><span class="sxs-lookup"><span data-stu-id="4c9d3-131">id</span></span>|<span data-ttu-id="4c9d3-132">String</span><span class="sxs-lookup"><span data-stu-id="4c9d3-132">String</span></span>|<span data-ttu-id="4c9d3-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4c9d3-133">Key of the entity.</span></span> <span data-ttu-id="4c9d3-134">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4c9d3-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4c9d3-135">displayName</span><span class="sxs-lookup"><span data-stu-id="4c9d3-135">displayName</span></span>|<span data-ttu-id="4c9d3-136">String</span><span class="sxs-lookup"><span data-stu-id="4c9d3-136">String</span></span>|<span data-ttu-id="4c9d3-137">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="4c9d3-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="4c9d3-138">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4c9d3-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4c9d3-139">descrição</span><span class="sxs-lookup"><span data-stu-id="4c9d3-139">description</span></span>|<span data-ttu-id="4c9d3-140">String</span><span class="sxs-lookup"><span data-stu-id="4c9d3-140">String</span></span>|<span data-ttu-id="4c9d3-141">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4c9d3-141">The description of the app.</span></span> <span data-ttu-id="4c9d3-142">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4c9d3-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4c9d3-143">publicador</span><span class="sxs-lookup"><span data-stu-id="4c9d3-143">publisher</span></span>|<span data-ttu-id="4c9d3-144">String</span><span class="sxs-lookup"><span data-stu-id="4c9d3-144">String</span></span>|<span data-ttu-id="4c9d3-145">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4c9d3-145">The publisher of the app.</span></span> <span data-ttu-id="4c9d3-146">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4c9d3-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4c9d3-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="4c9d3-147">largeIcon</span></span>|[<span data-ttu-id="4c9d3-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="4c9d3-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="4c9d3-149">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="4c9d3-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="4c9d3-150">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4c9d3-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4c9d3-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4c9d3-151">createdDateTime</span></span>|<span data-ttu-id="4c9d3-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c9d3-152">DateTimeOffset</span></span>|<span data-ttu-id="4c9d3-153">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4c9d3-153">The date and time the app was created.</span></span> <span data-ttu-id="4c9d3-154">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4c9d3-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4c9d3-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4c9d3-155">lastModifiedDateTime</span></span>|<span data-ttu-id="4c9d3-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c9d3-156">DateTimeOffset</span></span>|<span data-ttu-id="4c9d3-157">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="4c9d3-157">The date and time the app was last modified.</span></span> <span data-ttu-id="4c9d3-158">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4c9d3-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4c9d3-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="4c9d3-159">isFeatured</span></span>|<span data-ttu-id="4c9d3-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c9d3-160">Boolean</span></span>|<span data-ttu-id="4c9d3-161">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4c9d3-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4c9d3-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="4c9d3-162">privacyInformationUrl</span></span>|<span data-ttu-id="4c9d3-163">String</span><span class="sxs-lookup"><span data-stu-id="4c9d3-163">String</span></span>|<span data-ttu-id="4c9d3-164">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="4c9d3-164">The privacy statement Url.</span></span> <span data-ttu-id="4c9d3-165">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4c9d3-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4c9d3-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="4c9d3-166">informationUrl</span></span>|<span data-ttu-id="4c9d3-167">String</span><span class="sxs-lookup"><span data-stu-id="4c9d3-167">String</span></span>|<span data-ttu-id="4c9d3-168">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="4c9d3-168">The more information Url.</span></span> <span data-ttu-id="4c9d3-169">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4c9d3-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4c9d3-170">owner</span><span class="sxs-lookup"><span data-stu-id="4c9d3-170">owner</span></span>|<span data-ttu-id="4c9d3-171">String</span><span class="sxs-lookup"><span data-stu-id="4c9d3-171">String</span></span>|<span data-ttu-id="4c9d3-172">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="4c9d3-172">The owner of the app.</span></span> <span data-ttu-id="4c9d3-173">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4c9d3-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4c9d3-174">developer</span><span class="sxs-lookup"><span data-stu-id="4c9d3-174">developer</span></span>|<span data-ttu-id="4c9d3-175">String</span><span class="sxs-lookup"><span data-stu-id="4c9d3-175">String</span></span>|<span data-ttu-id="4c9d3-176">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4c9d3-176">The developer of the app.</span></span> <span data-ttu-id="4c9d3-177">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4c9d3-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4c9d3-178">notes</span><span class="sxs-lookup"><span data-stu-id="4c9d3-178">notes</span></span>|<span data-ttu-id="4c9d3-179">String</span><span class="sxs-lookup"><span data-stu-id="4c9d3-179">String</span></span>|<span data-ttu-id="4c9d3-180">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4c9d3-180">Notes for the app.</span></span> <span data-ttu-id="4c9d3-181">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4c9d3-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4c9d3-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="4c9d3-182">publishingState</span></span>|[<span data-ttu-id="4c9d3-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="4c9d3-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="4c9d3-184">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4c9d3-184">The publishing state for the app.</span></span> <span data-ttu-id="4c9d3-185">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="4c9d3-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="4c9d3-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4c9d3-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="4c9d3-187">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="4c9d3-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="4c9d3-188">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="4c9d3-188">usedLicenseCount</span></span>|<span data-ttu-id="4c9d3-189">Int32</span><span class="sxs-lookup"><span data-stu-id="4c9d3-189">Int32</span></span>|<span data-ttu-id="4c9d3-190">O número de aplicativos da Microsoft Store for Business em uso.</span><span class="sxs-lookup"><span data-stu-id="4c9d3-190">The number of Microsoft Store for Business licenses in use.</span></span>|
|<span data-ttu-id="4c9d3-191">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="4c9d3-191">totalLicenseCount</span></span>|<span data-ttu-id="4c9d3-192">Int32</span><span class="sxs-lookup"><span data-stu-id="4c9d3-192">Int32</span></span>|<span data-ttu-id="4c9d3-193">O número total de aplicativos da Microsoft Store for Business.</span><span class="sxs-lookup"><span data-stu-id="4c9d3-193">The total number of Microsoft Store for Business licenses.</span></span>|
|<span data-ttu-id="4c9d3-194">productKey</span><span class="sxs-lookup"><span data-stu-id="4c9d3-194">productKey</span></span>|<span data-ttu-id="4c9d3-195">String</span><span class="sxs-lookup"><span data-stu-id="4c9d3-195">String</span></span>|<span data-ttu-id="4c9d3-196">A chave de produto do aplicativo</span><span class="sxs-lookup"><span data-stu-id="4c9d3-196">The app product key</span></span>|
|<span data-ttu-id="4c9d3-197">licenseType</span><span class="sxs-lookup"><span data-stu-id="4c9d3-197">licenseType</span></span>|[<span data-ttu-id="4c9d3-198">microsoftStoreForBusinessLicenseType</span><span class="sxs-lookup"><span data-stu-id="4c9d3-198">microsoftStoreForBusinessLicenseType</span></span>](../resources/intune-apps-microsoftstoreforbusinesslicensetype.md)|<span data-ttu-id="4c9d3-199">O tipo de licença do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4c9d3-199">The app license type.</span></span> <span data-ttu-id="4c9d3-200">Os valores possíveis são: `offline` e `online`.</span><span class="sxs-lookup"><span data-stu-id="4c9d3-200">Possible values are: `offline`, `online`.</span></span>|
|<span data-ttu-id="4c9d3-201">packageIdentityName</span><span class="sxs-lookup"><span data-stu-id="4c9d3-201">packageIdentityName</span></span>|<span data-ttu-id="4c9d3-202">String</span><span class="sxs-lookup"><span data-stu-id="4c9d3-202">String</span></span>|<span data-ttu-id="4c9d3-203">O identificador do pacote do aplicativo</span><span class="sxs-lookup"><span data-stu-id="4c9d3-203">The app package identifier</span></span>|



## <a name="response"></a><span data-ttu-id="4c9d3-204">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c9d3-204">Response</span></span>
<span data-ttu-id="4c9d3-205">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4c9d3-205">If successful, this method returns a `200 OK` response code and an updated [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c9d3-206">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4c9d3-206">Example</span></span>

### <a name="request"></a><span data-ttu-id="4c9d3-207">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4c9d3-207">Request</span></span>
<span data-ttu-id="4c9d3-208">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4c9d3-208">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 769

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
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
  "publishingState": "processing",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "productKey": "Product Key value",
  "licenseType": "online",
  "packageIdentityName": "Package Identity Name value"
}
```

### <a name="response"></a><span data-ttu-id="4c9d3-209">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c9d3-209">Response</span></span>
<span data-ttu-id="4c9d3-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4c9d3-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 941

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
  "id": "f33358bc-58bc-f333-bc58-33f3bc5833f3",
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
  "publishingState": "processing",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "productKey": "Product Key value",
  "licenseType": "online",
  "packageIdentityName": "Package Identity Name value"
}
```



