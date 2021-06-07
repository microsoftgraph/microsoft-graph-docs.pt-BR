---
title: Atualizar iosStoreApp
description: Atualiza as propriedades de um objeto iosStoreApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6577ba56d424b477557f198458a73b64bafa6f92
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757329"
---
# <a name="update-iosstoreapp"></a><span data-ttu-id="f7201-103">Atualizar iosStoreApp</span><span class="sxs-lookup"><span data-stu-id="f7201-103">Update iosStoreApp</span></span>

<span data-ttu-id="f7201-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7201-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f7201-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f7201-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7201-106">Atualiza as propriedades de um objeto [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="f7201-106">Update the properties of a [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f7201-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f7201-107">Prerequisites</span></span>
<span data-ttu-id="f7201-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7201-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7201-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f7201-110">Permission type</span></span>|<span data-ttu-id="f7201-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f7201-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f7201-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f7201-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f7201-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7201-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f7201-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f7201-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7201-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f7201-115">Not supported.</span></span>|
|<span data-ttu-id="f7201-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f7201-116">Application</span></span>|<span data-ttu-id="f7201-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7201-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f7201-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f7201-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="f7201-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f7201-119">Request headers</span></span>
|<span data-ttu-id="f7201-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f7201-120">Header</span></span>|<span data-ttu-id="f7201-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f7201-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f7201-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f7201-122">Authorization</span></span>|<span data-ttu-id="f7201-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f7201-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f7201-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f7201-124">Accept</span></span>|<span data-ttu-id="f7201-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f7201-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7201-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f7201-126">Request body</span></span>
<span data-ttu-id="f7201-127">No corpo da solicitação, forneça uma representação JSON do objeto [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="f7201-127">In the request body, supply a JSON representation for the [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object.</span></span>

<span data-ttu-id="f7201-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="f7201-128">The following table shows the properties that are required when you create the [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span></span>

|<span data-ttu-id="f7201-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f7201-129">Property</span></span>|<span data-ttu-id="f7201-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f7201-130">Type</span></span>|<span data-ttu-id="f7201-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7201-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7201-132">id</span><span class="sxs-lookup"><span data-stu-id="f7201-132">id</span></span>|<span data-ttu-id="f7201-133">String</span><span class="sxs-lookup"><span data-stu-id="f7201-133">String</span></span>|<span data-ttu-id="f7201-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f7201-134">Key of the entity.</span></span> <span data-ttu-id="f7201-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f7201-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f7201-136">displayName</span><span class="sxs-lookup"><span data-stu-id="f7201-136">displayName</span></span>|<span data-ttu-id="f7201-137">String</span><span class="sxs-lookup"><span data-stu-id="f7201-137">String</span></span>|<span data-ttu-id="f7201-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="f7201-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="f7201-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f7201-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f7201-140">description</span><span class="sxs-lookup"><span data-stu-id="f7201-140">description</span></span>|<span data-ttu-id="f7201-141">String</span><span class="sxs-lookup"><span data-stu-id="f7201-141">String</span></span>|<span data-ttu-id="f7201-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f7201-142">The description of the app.</span></span> <span data-ttu-id="f7201-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f7201-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f7201-144">publicador</span><span class="sxs-lookup"><span data-stu-id="f7201-144">publisher</span></span>|<span data-ttu-id="f7201-145">String</span><span class="sxs-lookup"><span data-stu-id="f7201-145">String</span></span>|<span data-ttu-id="f7201-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f7201-146">The publisher of the app.</span></span> <span data-ttu-id="f7201-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f7201-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f7201-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="f7201-148">largeIcon</span></span>|[<span data-ttu-id="f7201-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f7201-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f7201-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="f7201-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="f7201-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f7201-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f7201-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f7201-152">createdDateTime</span></span>|<span data-ttu-id="f7201-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7201-153">DateTimeOffset</span></span>|<span data-ttu-id="f7201-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f7201-154">The date and time the app was created.</span></span> <span data-ttu-id="f7201-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f7201-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f7201-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f7201-156">lastModifiedDateTime</span></span>|<span data-ttu-id="f7201-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7201-157">DateTimeOffset</span></span>|<span data-ttu-id="f7201-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="f7201-158">The date and time the app was last modified.</span></span> <span data-ttu-id="f7201-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f7201-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f7201-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="f7201-160">isFeatured</span></span>|<span data-ttu-id="f7201-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="f7201-161">Boolean</span></span>|<span data-ttu-id="f7201-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f7201-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f7201-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f7201-163">privacyInformationUrl</span></span>|<span data-ttu-id="f7201-164">String</span><span class="sxs-lookup"><span data-stu-id="f7201-164">String</span></span>|<span data-ttu-id="f7201-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="f7201-165">The privacy statement Url.</span></span> <span data-ttu-id="f7201-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f7201-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f7201-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f7201-167">informationUrl</span></span>|<span data-ttu-id="f7201-168">String</span><span class="sxs-lookup"><span data-stu-id="f7201-168">String</span></span>|<span data-ttu-id="f7201-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="f7201-169">The more information Url.</span></span> <span data-ttu-id="f7201-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f7201-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f7201-171">proprietário</span><span class="sxs-lookup"><span data-stu-id="f7201-171">owner</span></span>|<span data-ttu-id="f7201-172">String</span><span class="sxs-lookup"><span data-stu-id="f7201-172">String</span></span>|<span data-ttu-id="f7201-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="f7201-173">The owner of the app.</span></span> <span data-ttu-id="f7201-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f7201-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f7201-175">developer</span><span class="sxs-lookup"><span data-stu-id="f7201-175">developer</span></span>|<span data-ttu-id="f7201-176">String</span><span class="sxs-lookup"><span data-stu-id="f7201-176">String</span></span>|<span data-ttu-id="f7201-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f7201-177">The developer of the app.</span></span> <span data-ttu-id="f7201-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f7201-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f7201-179">notes</span><span class="sxs-lookup"><span data-stu-id="f7201-179">notes</span></span>|<span data-ttu-id="f7201-180">String</span><span class="sxs-lookup"><span data-stu-id="f7201-180">String</span></span>|<span data-ttu-id="f7201-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f7201-181">Notes for the app.</span></span> <span data-ttu-id="f7201-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f7201-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f7201-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="f7201-183">publishingState</span></span>|[<span data-ttu-id="f7201-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="f7201-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="f7201-185">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f7201-185">The publishing state for the app.</span></span> <span data-ttu-id="f7201-186">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="f7201-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="f7201-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f7201-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="f7201-188">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="f7201-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="f7201-189">bundleId</span><span class="sxs-lookup"><span data-stu-id="f7201-189">bundleId</span></span>|<span data-ttu-id="f7201-190">String</span><span class="sxs-lookup"><span data-stu-id="f7201-190">String</span></span>|<span data-ttu-id="f7201-191">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="f7201-191">The Identity Name.</span></span>|
|<span data-ttu-id="f7201-192">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="f7201-192">appStoreUrl</span></span>|<span data-ttu-id="f7201-193">String</span><span class="sxs-lookup"><span data-stu-id="f7201-193">String</span></span>|<span data-ttu-id="f7201-194">A URL da Apple App Store</span><span class="sxs-lookup"><span data-stu-id="f7201-194">The Apple App Store URL</span></span>|
|<span data-ttu-id="f7201-195">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="f7201-195">applicableDeviceType</span></span>|[<span data-ttu-id="f7201-196">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="f7201-196">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="f7201-197">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="f7201-197">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="f7201-198">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f7201-198">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="f7201-199">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f7201-199">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="f7201-200">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="f7201-200">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="f7201-201">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7201-201">Response</span></span>
<span data-ttu-id="f7201-202">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [iosStoreApp](../resources/intune-apps-iosstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f7201-202">If successful, this method returns a `200 OK` response code and an updated [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7201-203">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f7201-203">Example</span></span>

### <a name="request"></a><span data-ttu-id="f7201-204">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f7201-204">Request</span></span>
<span data-ttu-id="f7201-205">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f7201-205">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1046

{
  "@odata.type": "#microsoft.graph.iosStoreApp",
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
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true,
    "v13_0": true,
    "v14_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="f7201-206">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7201-206">Response</span></span>
<span data-ttu-id="f7201-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f7201-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1218

{
  "@odata.type": "#microsoft.graph.iosStoreApp",
  "id": "a04adbe2-dbe2-a04a-e2db-4aa0e2db4aa0",
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
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true,
    "v13_0": true,
    "v14_0": true
  }
}
```




