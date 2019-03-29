---
title: Atualizar iosStoreApp
description: Atualiza as propriedades de um objeto iosStoreApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a4ad218975d5d4b6ac23e294a3321635ff415d69
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30979554"
---
# <a name="update-iosstoreapp"></a><span data-ttu-id="b8af7-103">Atualizar iosStoreApp</span><span class="sxs-lookup"><span data-stu-id="b8af7-103">Update iosStoreApp</span></span>

> <span data-ttu-id="b8af7-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b8af7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8af7-105">Atualiza as propriedades de um objeto [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="b8af7-105">Update the properties of a [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b8af7-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b8af7-106">Prerequisites</span></span>
<span data-ttu-id="b8af7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8af7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8af7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b8af7-109">Permission type</span></span>|<span data-ttu-id="b8af7-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b8af7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8af7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b8af7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b8af7-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8af7-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b8af7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b8af7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8af7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8af7-114">Not supported.</span></span>|
|<span data-ttu-id="b8af7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b8af7-115">Application</span></span>|<span data-ttu-id="b8af7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8af7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8af7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b8af7-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="b8af7-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b8af7-118">Request headers</span></span>
|<span data-ttu-id="b8af7-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b8af7-119">Header</span></span>|<span data-ttu-id="b8af7-120">Valor</span><span class="sxs-lookup"><span data-stu-id="b8af7-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b8af7-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b8af7-121">Authorization</span></span>|<span data-ttu-id="b8af7-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b8af7-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b8af7-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b8af7-123">Accept</span></span>|<span data-ttu-id="b8af7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b8af7-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8af7-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b8af7-125">Request body</span></span>
<span data-ttu-id="b8af7-126">No corpo da solicitação, forneça uma representação JSON do objeto [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="b8af7-126">In the request body, supply a JSON representation for the [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object.</span></span>

<span data-ttu-id="b8af7-127">A tabela a seguir mostra as propriedades obrigatórias ao criar [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="b8af7-127">The following table shows the properties that are required when you create the [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span></span>

|<span data-ttu-id="b8af7-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b8af7-128">Property</span></span>|<span data-ttu-id="b8af7-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="b8af7-129">Type</span></span>|<span data-ttu-id="b8af7-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8af7-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8af7-131">id</span><span class="sxs-lookup"><span data-stu-id="b8af7-131">id</span></span>|<span data-ttu-id="b8af7-132">String</span><span class="sxs-lookup"><span data-stu-id="b8af7-132">String</span></span>|<span data-ttu-id="b8af7-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b8af7-133">Key of the entity.</span></span> <span data-ttu-id="b8af7-134">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b8af7-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b8af7-135">displayName</span><span class="sxs-lookup"><span data-stu-id="b8af7-135">displayName</span></span>|<span data-ttu-id="b8af7-136">String</span><span class="sxs-lookup"><span data-stu-id="b8af7-136">String</span></span>|<span data-ttu-id="b8af7-137">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="b8af7-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="b8af7-138">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b8af7-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b8af7-139">descrição</span><span class="sxs-lookup"><span data-stu-id="b8af7-139">description</span></span>|<span data-ttu-id="b8af7-140">String</span><span class="sxs-lookup"><span data-stu-id="b8af7-140">String</span></span>|<span data-ttu-id="b8af7-141">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b8af7-141">The description of the app.</span></span> <span data-ttu-id="b8af7-142">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b8af7-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b8af7-143">publicador</span><span class="sxs-lookup"><span data-stu-id="b8af7-143">publisher</span></span>|<span data-ttu-id="b8af7-144">String</span><span class="sxs-lookup"><span data-stu-id="b8af7-144">String</span></span>|<span data-ttu-id="b8af7-145">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b8af7-145">The publisher of the app.</span></span> <span data-ttu-id="b8af7-146">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b8af7-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b8af7-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="b8af7-147">largeIcon</span></span>|[<span data-ttu-id="b8af7-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b8af7-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="b8af7-149">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="b8af7-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="b8af7-150">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b8af7-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b8af7-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b8af7-151">createdDateTime</span></span>|<span data-ttu-id="b8af7-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8af7-152">DateTimeOffset</span></span>|<span data-ttu-id="b8af7-153">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b8af7-153">The date and time the app was created.</span></span> <span data-ttu-id="b8af7-154">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b8af7-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b8af7-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b8af7-155">lastModifiedDateTime</span></span>|<span data-ttu-id="b8af7-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8af7-156">DateTimeOffset</span></span>|<span data-ttu-id="b8af7-157">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="b8af7-157">The date and time the app was last modified.</span></span> <span data-ttu-id="b8af7-158">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b8af7-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b8af7-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="b8af7-159">isFeatured</span></span>|<span data-ttu-id="b8af7-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="b8af7-160">Boolean</span></span>|<span data-ttu-id="b8af7-161">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b8af7-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b8af7-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="b8af7-162">privacyInformationUrl</span></span>|<span data-ttu-id="b8af7-163">String</span><span class="sxs-lookup"><span data-stu-id="b8af7-163">String</span></span>|<span data-ttu-id="b8af7-164">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="b8af7-164">The privacy statement Url.</span></span> <span data-ttu-id="b8af7-165">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b8af7-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b8af7-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="b8af7-166">informationUrl</span></span>|<span data-ttu-id="b8af7-167">String</span><span class="sxs-lookup"><span data-stu-id="b8af7-167">String</span></span>|<span data-ttu-id="b8af7-168">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="b8af7-168">The more information Url.</span></span> <span data-ttu-id="b8af7-169">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b8af7-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b8af7-170">owner</span><span class="sxs-lookup"><span data-stu-id="b8af7-170">owner</span></span>|<span data-ttu-id="b8af7-171">String</span><span class="sxs-lookup"><span data-stu-id="b8af7-171">String</span></span>|<span data-ttu-id="b8af7-172">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="b8af7-172">The owner of the app.</span></span> <span data-ttu-id="b8af7-173">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b8af7-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b8af7-174">developer</span><span class="sxs-lookup"><span data-stu-id="b8af7-174">developer</span></span>|<span data-ttu-id="b8af7-175">String</span><span class="sxs-lookup"><span data-stu-id="b8af7-175">String</span></span>|<span data-ttu-id="b8af7-176">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b8af7-176">The developer of the app.</span></span> <span data-ttu-id="b8af7-177">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b8af7-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b8af7-178">notes</span><span class="sxs-lookup"><span data-stu-id="b8af7-178">notes</span></span>|<span data-ttu-id="b8af7-179">String</span><span class="sxs-lookup"><span data-stu-id="b8af7-179">String</span></span>|<span data-ttu-id="b8af7-180">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b8af7-180">Notes for the app.</span></span> <span data-ttu-id="b8af7-181">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b8af7-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b8af7-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="b8af7-182">publishingState</span></span>|[<span data-ttu-id="b8af7-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="b8af7-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="b8af7-184">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b8af7-184">The publishing state for the app.</span></span> <span data-ttu-id="b8af7-185">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="b8af7-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="b8af7-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b8af7-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="b8af7-187">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="b8af7-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="b8af7-188">bundleId</span><span class="sxs-lookup"><span data-stu-id="b8af7-188">bundleId</span></span>|<span data-ttu-id="b8af7-189">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b8af7-189">String</span></span>|<span data-ttu-id="b8af7-190">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="b8af7-190">The Identity Name.</span></span>|
|<span data-ttu-id="b8af7-191">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="b8af7-191">appStoreUrl</span></span>|<span data-ttu-id="b8af7-192">String</span><span class="sxs-lookup"><span data-stu-id="b8af7-192">String</span></span>|<span data-ttu-id="b8af7-193">A URL da Apple App Store</span><span class="sxs-lookup"><span data-stu-id="b8af7-193">The Apple App Store URL</span></span>|
|<span data-ttu-id="b8af7-194">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="b8af7-194">applicableDeviceType</span></span>|[<span data-ttu-id="b8af7-195">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="b8af7-195">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="b8af7-196">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="b8af7-196">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="b8af7-197">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b8af7-197">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="b8af7-198">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b8af7-198">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="b8af7-199">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="b8af7-199">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="b8af7-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8af7-200">Response</span></span>
<span data-ttu-id="b8af7-201">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [iosStoreApp](../resources/intune-apps-iosstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b8af7-201">If successful, this method returns a `200 OK` response code and an updated [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8af7-202">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b8af7-202">Example</span></span>

### <a name="request"></a><span data-ttu-id="b8af7-203">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b8af7-203">Request</span></span>
<span data-ttu-id="b8af7-204">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b8af7-204">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1006

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
    "v12_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="b8af7-205">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8af7-205">Response</span></span>
<span data-ttu-id="b8af7-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b8af7-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1178

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
    "v12_0": true
  }
}
```



