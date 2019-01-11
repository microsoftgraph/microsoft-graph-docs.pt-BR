---
title: Criar androidStoreApp
description: Criar um novo objeto androidStoreApp.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 73513177a83734618c01e9bd03282f1e20f9efa7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814585"
---
# <a name="create-androidstoreapp"></a><span data-ttu-id="3d7c2-103">Criar androidStoreApp</span><span class="sxs-lookup"><span data-stu-id="3d7c2-103">Create androidStoreApp</span></span>

> <span data-ttu-id="3d7c2-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3d7c2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3d7c2-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3d7c2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3d7c2-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3d7c2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3d7c2-107">Criar um novo objeto [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="3d7c2-107">Create a new [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3d7c2-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3d7c2-108">Prerequisites</span></span>
<span data-ttu-id="3d7c2-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d7c2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d7c2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3d7c2-111">Permission type</span></span>|<span data-ttu-id="3d7c2-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3d7c2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3d7c2-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3d7c2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3d7c2-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d7c2-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3d7c2-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3d7c2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3d7c2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3d7c2-116">Not supported.</span></span>|
|<span data-ttu-id="3d7c2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3d7c2-117">Application</span></span>|<span data-ttu-id="3d7c2-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3d7c2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3d7c2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3d7c2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="3d7c2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3d7c2-120">Request headers</span></span>
|<span data-ttu-id="3d7c2-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3d7c2-121">Header</span></span>|<span data-ttu-id="3d7c2-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3d7c2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3d7c2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3d7c2-123">Authorization</span></span>|<span data-ttu-id="3d7c2-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3d7c2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3d7c2-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3d7c2-125">Accept</span></span>|<span data-ttu-id="3d7c2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3d7c2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d7c2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3d7c2-127">Request body</span></span>
<span data-ttu-id="3d7c2-128">No corpo da solicitação, forneça uma representação JSON do objeto androidStoreApp.</span><span class="sxs-lookup"><span data-stu-id="3d7c2-128">In the request body, supply a JSON representation for the androidStoreApp object.</span></span>

<span data-ttu-id="3d7c2-129">A tabela a seguir mostra as propriedades que são necessárias ao criar androidStoreApp.</span><span class="sxs-lookup"><span data-stu-id="3d7c2-129">The following table shows the properties that are required when you create the androidStoreApp.</span></span>

|<span data-ttu-id="3d7c2-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3d7c2-130">Property</span></span>|<span data-ttu-id="3d7c2-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3d7c2-131">Type</span></span>|<span data-ttu-id="3d7c2-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d7c2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d7c2-133">id</span><span class="sxs-lookup"><span data-stu-id="3d7c2-133">id</span></span>|<span data-ttu-id="3d7c2-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3d7c2-134">String</span></span>|<span data-ttu-id="3d7c2-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3d7c2-135">Key of the entity.</span></span> <span data-ttu-id="3d7c2-136">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3d7c2-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3d7c2-137">displayName</span><span class="sxs-lookup"><span data-stu-id="3d7c2-137">displayName</span></span>|<span data-ttu-id="3d7c2-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3d7c2-138">String</span></span>|<span data-ttu-id="3d7c2-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="3d7c2-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="3d7c2-140">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3d7c2-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3d7c2-141">description</span><span class="sxs-lookup"><span data-stu-id="3d7c2-141">description</span></span>|<span data-ttu-id="3d7c2-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3d7c2-142">String</span></span>|<span data-ttu-id="3d7c2-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3d7c2-143">The description of the app.</span></span> <span data-ttu-id="3d7c2-144">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3d7c2-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3d7c2-145">publisher</span><span class="sxs-lookup"><span data-stu-id="3d7c2-145">publisher</span></span>|<span data-ttu-id="3d7c2-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3d7c2-146">String</span></span>|<span data-ttu-id="3d7c2-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3d7c2-147">The publisher of the app.</span></span> <span data-ttu-id="3d7c2-148">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3d7c2-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3d7c2-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="3d7c2-149">largeIcon</span></span>|[<span data-ttu-id="3d7c2-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="3d7c2-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="3d7c2-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="3d7c2-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="3d7c2-152">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3d7c2-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3d7c2-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3d7c2-153">createdDateTime</span></span>|<span data-ttu-id="3d7c2-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d7c2-154">DateTimeOffset</span></span>|<span data-ttu-id="3d7c2-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3d7c2-155">The date and time the app was created.</span></span> <span data-ttu-id="3d7c2-156">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3d7c2-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3d7c2-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3d7c2-157">lastModifiedDateTime</span></span>|<span data-ttu-id="3d7c2-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d7c2-158">DateTimeOffset</span></span>|<span data-ttu-id="3d7c2-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="3d7c2-159">The date and time the app was last modified.</span></span> <span data-ttu-id="3d7c2-160">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3d7c2-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3d7c2-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="3d7c2-161">isFeatured</span></span>|<span data-ttu-id="3d7c2-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="3d7c2-162">Boolean</span></span>|<span data-ttu-id="3d7c2-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3d7c2-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3d7c2-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="3d7c2-164">privacyInformationUrl</span></span>|<span data-ttu-id="3d7c2-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3d7c2-165">String</span></span>|<span data-ttu-id="3d7c2-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="3d7c2-166">The privacy statement Url.</span></span> <span data-ttu-id="3d7c2-167">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3d7c2-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3d7c2-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="3d7c2-168">informationUrl</span></span>|<span data-ttu-id="3d7c2-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3d7c2-169">String</span></span>|<span data-ttu-id="3d7c2-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="3d7c2-170">The more information Url.</span></span> <span data-ttu-id="3d7c2-171">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3d7c2-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3d7c2-172">owner</span><span class="sxs-lookup"><span data-stu-id="3d7c2-172">owner</span></span>|<span data-ttu-id="3d7c2-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3d7c2-173">String</span></span>|<span data-ttu-id="3d7c2-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="3d7c2-174">The owner of the app.</span></span> <span data-ttu-id="3d7c2-175">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3d7c2-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3d7c2-176">developer</span><span class="sxs-lookup"><span data-stu-id="3d7c2-176">developer</span></span>|<span data-ttu-id="3d7c2-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3d7c2-177">String</span></span>|<span data-ttu-id="3d7c2-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3d7c2-178">The developer of the app.</span></span> <span data-ttu-id="3d7c2-179">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3d7c2-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3d7c2-180">Observações</span><span class="sxs-lookup"><span data-stu-id="3d7c2-180">notes</span></span>|<span data-ttu-id="3d7c2-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3d7c2-181">String</span></span>|<span data-ttu-id="3d7c2-182">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3d7c2-182">Notes for the app.</span></span> <span data-ttu-id="3d7c2-183">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3d7c2-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3d7c2-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="3d7c2-184">uploadState</span></span>|<span data-ttu-id="3d7c2-185">Int32</span><span class="sxs-lookup"><span data-stu-id="3d7c2-185">Int32</span></span>|<span data-ttu-id="3d7c2-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="3d7c2-186">The upload state.</span></span> <span data-ttu-id="3d7c2-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3d7c2-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3d7c2-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="3d7c2-188">publishingState</span></span>|[<span data-ttu-id="3d7c2-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="3d7c2-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="3d7c2-190">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3d7c2-190">The publishing state for the app.</span></span> <span data-ttu-id="3d7c2-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="3d7c2-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="3d7c2-192">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3d7c2-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="3d7c2-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="3d7c2-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="3d7c2-194">packageId</span><span class="sxs-lookup"><span data-stu-id="3d7c2-194">packageId</span></span>|<span data-ttu-id="3d7c2-195">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3d7c2-195">String</span></span>|<span data-ttu-id="3d7c2-196">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="3d7c2-196">The package identifier.</span></span>|
|<span data-ttu-id="3d7c2-197">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="3d7c2-197">appIdentifier</span></span>|<span data-ttu-id="3d7c2-198">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3d7c2-198">String</span></span>|<span data-ttu-id="3d7c2-199">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="3d7c2-199">The Identity Name.</span></span>|
|<span data-ttu-id="3d7c2-200">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="3d7c2-200">appStoreUrl</span></span>|<span data-ttu-id="3d7c2-201">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3d7c2-201">String</span></span>|<span data-ttu-id="3d7c2-202">A URL da loja de aplicativos Android.</span><span class="sxs-lookup"><span data-stu-id="3d7c2-202">The Android app store URL.</span></span>|
|<span data-ttu-id="3d7c2-203">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="3d7c2-203">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="3d7c2-204">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="3d7c2-204">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="3d7c2-205">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="3d7c2-205">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="3d7c2-206">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d7c2-206">Response</span></span>
<span data-ttu-id="3d7c2-207">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [androidStoreApp](../resources/intune-apps-androidstoreapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3d7c2-207">If successful, this method returns a `201 Created` response code and a [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d7c2-208">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3d7c2-208">Example</span></span>
### <a name="request"></a><span data-ttu-id="3d7c2-209">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3d7c2-209">Request</span></span>
<span data-ttu-id="3d7c2-210">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3d7c2-210">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1182

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

### <a name="response"></a><span data-ttu-id="3d7c2-211">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d7c2-211">Response</span></span>
<span data-ttu-id="3d7c2-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3d7c2-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1290

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





