---
title: Criar androidManagedStoreApp
description: Crie um novo objeto de androidManagedStoreApp.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 37e59470f8c1bf5cd740aa9ce4d6a09c13a7d5b5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27930492"
---
# <a name="create-androidmanagedstoreapp"></a><span data-ttu-id="73064-103">Criar androidManagedStoreApp</span><span class="sxs-lookup"><span data-stu-id="73064-103">Create androidManagedStoreApp</span></span>

> <span data-ttu-id="73064-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="73064-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="73064-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="73064-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="73064-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="73064-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="73064-107">Crie um novo objeto de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) .</span><span class="sxs-lookup"><span data-stu-id="73064-107">Create a new [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="73064-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="73064-108">Prerequisites</span></span>
<span data-ttu-id="73064-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73064-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73064-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="73064-111">Permission type</span></span>|<span data-ttu-id="73064-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="73064-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73064-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="73064-113">Delegated (work or school account)</span></span>|<span data-ttu-id="73064-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73064-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="73064-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="73064-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73064-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="73064-116">Not supported.</span></span>|
|<span data-ttu-id="73064-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="73064-117">Application</span></span>|<span data-ttu-id="73064-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="73064-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="73064-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="73064-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="73064-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="73064-120">Request headers</span></span>
|<span data-ttu-id="73064-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="73064-121">Header</span></span>|<span data-ttu-id="73064-122">Valor</span><span class="sxs-lookup"><span data-stu-id="73064-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73064-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="73064-123">Authorization</span></span>|<span data-ttu-id="73064-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="73064-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="73064-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="73064-125">Accept</span></span>|<span data-ttu-id="73064-126">application/json</span><span class="sxs-lookup"><span data-stu-id="73064-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73064-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="73064-127">Request body</span></span>
<span data-ttu-id="73064-128">No corpo da solicitação, fornece uma representação JSON para o objeto androidManagedStoreApp.</span><span class="sxs-lookup"><span data-stu-id="73064-128">In the request body, supply a JSON representation for the androidManagedStoreApp object.</span></span>

<span data-ttu-id="73064-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o androidManagedStoreApp.</span><span class="sxs-lookup"><span data-stu-id="73064-129">The following table shows the properties that are required when you create the androidManagedStoreApp.</span></span>

|<span data-ttu-id="73064-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="73064-130">Property</span></span>|<span data-ttu-id="73064-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="73064-131">Type</span></span>|<span data-ttu-id="73064-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="73064-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73064-133">id</span><span class="sxs-lookup"><span data-stu-id="73064-133">id</span></span>|<span data-ttu-id="73064-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73064-134">String</span></span>|<span data-ttu-id="73064-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="73064-135">Key of the entity.</span></span> <span data-ttu-id="73064-136">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="73064-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="73064-137">displayName</span><span class="sxs-lookup"><span data-stu-id="73064-137">displayName</span></span>|<span data-ttu-id="73064-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73064-138">String</span></span>|<span data-ttu-id="73064-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="73064-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="73064-140">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="73064-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="73064-141">description</span><span class="sxs-lookup"><span data-stu-id="73064-141">description</span></span>|<span data-ttu-id="73064-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73064-142">String</span></span>|<span data-ttu-id="73064-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="73064-143">The description of the app.</span></span> <span data-ttu-id="73064-144">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="73064-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="73064-145">publisher</span><span class="sxs-lookup"><span data-stu-id="73064-145">publisher</span></span>|<span data-ttu-id="73064-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73064-146">String</span></span>|<span data-ttu-id="73064-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="73064-147">The publisher of the app.</span></span> <span data-ttu-id="73064-148">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="73064-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="73064-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="73064-149">largeIcon</span></span>|[<span data-ttu-id="73064-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="73064-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="73064-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="73064-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="73064-152">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="73064-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="73064-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="73064-153">createdDateTime</span></span>|<span data-ttu-id="73064-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73064-154">DateTimeOffset</span></span>|<span data-ttu-id="73064-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="73064-155">The date and time the app was created.</span></span> <span data-ttu-id="73064-156">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="73064-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="73064-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="73064-157">lastModifiedDateTime</span></span>|<span data-ttu-id="73064-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73064-158">DateTimeOffset</span></span>|<span data-ttu-id="73064-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="73064-159">The date and time the app was last modified.</span></span> <span data-ttu-id="73064-160">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="73064-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="73064-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="73064-161">isFeatured</span></span>|<span data-ttu-id="73064-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="73064-162">Boolean</span></span>|<span data-ttu-id="73064-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="73064-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="73064-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="73064-164">privacyInformationUrl</span></span>|<span data-ttu-id="73064-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73064-165">String</span></span>|<span data-ttu-id="73064-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="73064-166">The privacy statement Url.</span></span> <span data-ttu-id="73064-167">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="73064-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="73064-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="73064-168">informationUrl</span></span>|<span data-ttu-id="73064-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73064-169">String</span></span>|<span data-ttu-id="73064-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="73064-170">The more information Url.</span></span> <span data-ttu-id="73064-171">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="73064-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="73064-172">owner</span><span class="sxs-lookup"><span data-stu-id="73064-172">owner</span></span>|<span data-ttu-id="73064-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73064-173">String</span></span>|<span data-ttu-id="73064-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="73064-174">The owner of the app.</span></span> <span data-ttu-id="73064-175">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="73064-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="73064-176">developer</span><span class="sxs-lookup"><span data-stu-id="73064-176">developer</span></span>|<span data-ttu-id="73064-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73064-177">String</span></span>|<span data-ttu-id="73064-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="73064-178">The developer of the app.</span></span> <span data-ttu-id="73064-179">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="73064-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="73064-180">Observações</span><span class="sxs-lookup"><span data-stu-id="73064-180">notes</span></span>|<span data-ttu-id="73064-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73064-181">String</span></span>|<span data-ttu-id="73064-182">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="73064-182">Notes for the app.</span></span> <span data-ttu-id="73064-183">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="73064-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="73064-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="73064-184">uploadState</span></span>|<span data-ttu-id="73064-185">Int32</span><span class="sxs-lookup"><span data-stu-id="73064-185">Int32</span></span>|<span data-ttu-id="73064-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="73064-186">The upload state.</span></span> <span data-ttu-id="73064-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="73064-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="73064-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="73064-188">publishingState</span></span>|[<span data-ttu-id="73064-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="73064-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="73064-190">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="73064-190">The publishing state for the app.</span></span> <span data-ttu-id="73064-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="73064-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="73064-192">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="73064-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="73064-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="73064-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="73064-194">packageId</span><span class="sxs-lookup"><span data-stu-id="73064-194">packageId</span></span>|<span data-ttu-id="73064-195">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73064-195">String</span></span>|<span data-ttu-id="73064-196">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="73064-196">The package identifier.</span></span>|
|<span data-ttu-id="73064-197">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="73064-197">appIdentifier</span></span>|<span data-ttu-id="73064-198">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73064-198">String</span></span>|<span data-ttu-id="73064-199">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="73064-199">The Identity Name.</span></span>|
|<span data-ttu-id="73064-200">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="73064-200">usedLicenseCount</span></span>|<span data-ttu-id="73064-201">Int32</span><span class="sxs-lookup"><span data-stu-id="73064-201">Int32</span></span>|<span data-ttu-id="73064-202">O número de aplicativos VPP em uso.</span><span class="sxs-lookup"><span data-stu-id="73064-202">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="73064-203">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="73064-203">totalLicenseCount</span></span>|<span data-ttu-id="73064-204">Int32</span><span class="sxs-lookup"><span data-stu-id="73064-204">Int32</span></span>|<span data-ttu-id="73064-205">O número total de licenças VPP.</span><span class="sxs-lookup"><span data-stu-id="73064-205">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="73064-206">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="73064-206">appStoreUrl</span></span>|<span data-ttu-id="73064-207">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73064-207">String</span></span>|<span data-ttu-id="73064-208">Tocar para a URL do aplicativo de repositório de trabalho.</span><span class="sxs-lookup"><span data-stu-id="73064-208">The Play for Work Store app URL.</span></span>|



## <a name="response"></a><span data-ttu-id="73064-209">Resposta</span><span class="sxs-lookup"><span data-stu-id="73064-209">Response</span></span>
<span data-ttu-id="73064-210">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="73064-210">If successful, this method returns a `201 Created` response code and a [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73064-211">Exemplo</span><span class="sxs-lookup"><span data-stu-id="73064-211">Example</span></span>
### <a name="request"></a><span data-ttu-id="73064-212">Solicitação</span><span class="sxs-lookup"><span data-stu-id="73064-212">Request</span></span>
<span data-ttu-id="73064-213">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="73064-213">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 860

{
  "@odata.type": "#microsoft.graph.androidManagedStoreApp",
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
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```

### <a name="response"></a><span data-ttu-id="73064-214">Resposta</span><span class="sxs-lookup"><span data-stu-id="73064-214">Response</span></span>
<span data-ttu-id="73064-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="73064-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 968

{
  "@odata.type": "#microsoft.graph.androidManagedStoreApp",
  "id": "87247525-7525-8724-2575-248725752487",
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
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```





