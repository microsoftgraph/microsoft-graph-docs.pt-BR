---
title: Atualizar microsoftStoreForBusinessApp
description: Atualiza as propriedades de um objeto microsoftStoreForBusinessApp.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e063091b1fde917ffa7b15607e74d425d2ebc29d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27960872"
---
# <a name="update-microsoftstoreforbusinessapp"></a><span data-ttu-id="18545-103">Atualizar microsoftStoreForBusinessApp</span><span class="sxs-lookup"><span data-stu-id="18545-103">Update microsoftStoreForBusinessApp</span></span>

> <span data-ttu-id="18545-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="18545-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="18545-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="18545-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="18545-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="18545-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="18545-107">Atualiza as propriedades de um objeto [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="18545-107">Update the properties of a [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="18545-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="18545-108">Prerequisites</span></span>
<span data-ttu-id="18545-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18545-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18545-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="18545-111">Permission type</span></span>|<span data-ttu-id="18545-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="18545-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18545-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="18545-113">Delegated (work or school account)</span></span>|<span data-ttu-id="18545-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18545-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="18545-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="18545-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18545-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="18545-116">Not supported.</span></span>|
|<span data-ttu-id="18545-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="18545-117">Application</span></span>|<span data-ttu-id="18545-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="18545-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="18545-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="18545-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="18545-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="18545-120">Request headers</span></span>
|<span data-ttu-id="18545-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="18545-121">Header</span></span>|<span data-ttu-id="18545-122">Valor</span><span class="sxs-lookup"><span data-stu-id="18545-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18545-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="18545-123">Authorization</span></span>|<span data-ttu-id="18545-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="18545-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18545-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="18545-125">Accept</span></span>|<span data-ttu-id="18545-126">application/json</span><span class="sxs-lookup"><span data-stu-id="18545-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18545-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="18545-127">Request body</span></span>
<span data-ttu-id="18545-128">No corpo da solicitação, forneça uma representação JSON do objeto [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="18545-128">In the request body, supply a JSON representation for the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

<span data-ttu-id="18545-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="18545-129">The following table shows the properties that are required when you create the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span></span>

|<span data-ttu-id="18545-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="18545-130">Property</span></span>|<span data-ttu-id="18545-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="18545-131">Type</span></span>|<span data-ttu-id="18545-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="18545-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18545-133">id</span><span class="sxs-lookup"><span data-stu-id="18545-133">id</span></span>|<span data-ttu-id="18545-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18545-134">String</span></span>|<span data-ttu-id="18545-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="18545-135">Key of the entity.</span></span> <span data-ttu-id="18545-136">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18545-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18545-137">displayName</span><span class="sxs-lookup"><span data-stu-id="18545-137">displayName</span></span>|<span data-ttu-id="18545-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18545-138">String</span></span>|<span data-ttu-id="18545-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="18545-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="18545-140">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18545-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18545-141">description</span><span class="sxs-lookup"><span data-stu-id="18545-141">description</span></span>|<span data-ttu-id="18545-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18545-142">String</span></span>|<span data-ttu-id="18545-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="18545-143">The description of the app.</span></span> <span data-ttu-id="18545-144">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18545-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18545-145">publisher</span><span class="sxs-lookup"><span data-stu-id="18545-145">publisher</span></span>|<span data-ttu-id="18545-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18545-146">String</span></span>|<span data-ttu-id="18545-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="18545-147">The publisher of the app.</span></span> <span data-ttu-id="18545-148">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18545-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18545-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="18545-149">largeIcon</span></span>|[<span data-ttu-id="18545-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="18545-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="18545-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="18545-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="18545-152">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18545-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18545-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="18545-153">createdDateTime</span></span>|<span data-ttu-id="18545-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18545-154">DateTimeOffset</span></span>|<span data-ttu-id="18545-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="18545-155">The date and time the app was created.</span></span> <span data-ttu-id="18545-156">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18545-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18545-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="18545-157">lastModifiedDateTime</span></span>|<span data-ttu-id="18545-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18545-158">DateTimeOffset</span></span>|<span data-ttu-id="18545-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="18545-159">The date and time the app was last modified.</span></span> <span data-ttu-id="18545-160">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18545-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18545-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="18545-161">isFeatured</span></span>|<span data-ttu-id="18545-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="18545-162">Boolean</span></span>|<span data-ttu-id="18545-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18545-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18545-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="18545-164">privacyInformationUrl</span></span>|<span data-ttu-id="18545-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18545-165">String</span></span>|<span data-ttu-id="18545-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="18545-166">The privacy statement Url.</span></span> <span data-ttu-id="18545-167">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18545-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18545-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="18545-168">informationUrl</span></span>|<span data-ttu-id="18545-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18545-169">String</span></span>|<span data-ttu-id="18545-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="18545-170">The more information Url.</span></span> <span data-ttu-id="18545-171">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18545-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18545-172">owner</span><span class="sxs-lookup"><span data-stu-id="18545-172">owner</span></span>|<span data-ttu-id="18545-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18545-173">String</span></span>|<span data-ttu-id="18545-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="18545-174">The owner of the app.</span></span> <span data-ttu-id="18545-175">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18545-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18545-176">developer</span><span class="sxs-lookup"><span data-stu-id="18545-176">developer</span></span>|<span data-ttu-id="18545-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18545-177">String</span></span>|<span data-ttu-id="18545-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="18545-178">The developer of the app.</span></span> <span data-ttu-id="18545-179">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18545-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18545-180">Observações</span><span class="sxs-lookup"><span data-stu-id="18545-180">notes</span></span>|<span data-ttu-id="18545-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18545-181">String</span></span>|<span data-ttu-id="18545-182">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="18545-182">Notes for the app.</span></span> <span data-ttu-id="18545-183">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18545-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18545-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="18545-184">uploadState</span></span>|<span data-ttu-id="18545-185">Int32</span><span class="sxs-lookup"><span data-stu-id="18545-185">Int32</span></span>|<span data-ttu-id="18545-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="18545-186">The upload state.</span></span> <span data-ttu-id="18545-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18545-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18545-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="18545-188">publishingState</span></span>|[<span data-ttu-id="18545-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="18545-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="18545-190">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="18545-190">The publishing state for the app.</span></span> <span data-ttu-id="18545-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="18545-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="18545-192">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="18545-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="18545-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="18545-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="18545-194">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="18545-194">usedLicenseCount</span></span>|<span data-ttu-id="18545-195">Int32</span><span class="sxs-lookup"><span data-stu-id="18545-195">Int32</span></span>|<span data-ttu-id="18545-196">O número de aplicativos da Microsoft Store for Business em uso.</span><span class="sxs-lookup"><span data-stu-id="18545-196">The number of Microsoft Store for Business licenses in use.</span></span>|
|<span data-ttu-id="18545-197">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="18545-197">totalLicenseCount</span></span>|<span data-ttu-id="18545-198">Int32</span><span class="sxs-lookup"><span data-stu-id="18545-198">Int32</span></span>|<span data-ttu-id="18545-199">O número total de aplicativos da Microsoft Store for Business.</span><span class="sxs-lookup"><span data-stu-id="18545-199">The total number of Microsoft Store for Business licenses.</span></span>|
|<span data-ttu-id="18545-200">productKey</span><span class="sxs-lookup"><span data-stu-id="18545-200">productKey</span></span>|<span data-ttu-id="18545-201">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18545-201">String</span></span>|<span data-ttu-id="18545-202">A chave de produto do aplicativo</span><span class="sxs-lookup"><span data-stu-id="18545-202">The app product key</span></span>|
|<span data-ttu-id="18545-203">licenseType</span><span class="sxs-lookup"><span data-stu-id="18545-203">licenseType</span></span>|[<span data-ttu-id="18545-204">microsoftStoreForBusinessLicenseType</span><span class="sxs-lookup"><span data-stu-id="18545-204">microsoftStoreForBusinessLicenseType</span></span>](../resources/intune-apps-microsoftstoreforbusinesslicensetype.md)|<span data-ttu-id="18545-205">O tipo de licença de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="18545-205">The app license type.</span></span> <span data-ttu-id="18545-206">Os valores possíveis são: `offline` e `online`.</span><span class="sxs-lookup"><span data-stu-id="18545-206">Possible values are: `offline`, `online`.</span></span>|
|<span data-ttu-id="18545-207">packageIdentityName</span><span class="sxs-lookup"><span data-stu-id="18545-207">packageIdentityName</span></span>|<span data-ttu-id="18545-208">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18545-208">String</span></span>|<span data-ttu-id="18545-209">O identificador do pacote do aplicativo</span><span class="sxs-lookup"><span data-stu-id="18545-209">The app package identifier</span></span>|



## <a name="response"></a><span data-ttu-id="18545-210">Resposta</span><span class="sxs-lookup"><span data-stu-id="18545-210">Response</span></span>
<span data-ttu-id="18545-211">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="18545-211">If successful, this method returns a `200 OK` response code and an updated [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18545-212">Exemplo</span><span class="sxs-lookup"><span data-stu-id="18545-212">Example</span></span>
### <a name="request"></a><span data-ttu-id="18545-213">Solicitação</span><span class="sxs-lookup"><span data-stu-id="18545-213">Request</span></span>
<span data-ttu-id="18545-214">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="18545-214">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 788

{
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "productKey": "Product Key value",
  "licenseType": "online",
  "packageIdentityName": "Package Identity Name value"
}
```

### <a name="response"></a><span data-ttu-id="18545-215">Resposta</span><span class="sxs-lookup"><span data-stu-id="18545-215">Response</span></span>
<span data-ttu-id="18545-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="18545-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 963

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
  "uploadState": 11,
  "publishingState": "processing",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "productKey": "Product Key value",
  "licenseType": "online",
  "packageIdentityName": "Package Identity Name value"
}
```





