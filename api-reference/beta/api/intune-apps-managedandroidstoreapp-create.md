---
title: Criar managedAndroidStoreApp
description: Cria um novo objeto managedAndroidStoreApp.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c0723230ebde8d4f06b759fcfe9b31aab669fe62
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819367"
---
# <a name="create-managedandroidstoreapp"></a><span data-ttu-id="8664e-103">Criar managedAndroidStoreApp</span><span class="sxs-lookup"><span data-stu-id="8664e-103">Create managedAndroidStoreApp</span></span>

> <span data-ttu-id="8664e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8664e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8664e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8664e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8664e-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8664e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8664e-107">Cria um novo objeto [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="8664e-107">Create a new [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8664e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8664e-108">Prerequisites</span></span>
<span data-ttu-id="8664e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8664e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8664e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8664e-111">Permission type</span></span>|<span data-ttu-id="8664e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8664e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8664e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8664e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8664e-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8664e-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8664e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8664e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8664e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8664e-116">Not supported.</span></span>|
|<span data-ttu-id="8664e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8664e-117">Application</span></span>|<span data-ttu-id="8664e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8664e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8664e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8664e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="8664e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8664e-120">Request headers</span></span>
|<span data-ttu-id="8664e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8664e-121">Header</span></span>|<span data-ttu-id="8664e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8664e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8664e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8664e-123">Authorization</span></span>|<span data-ttu-id="8664e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8664e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8664e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8664e-125">Accept</span></span>|<span data-ttu-id="8664e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8664e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8664e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8664e-127">Request body</span></span>
<span data-ttu-id="8664e-128">No corpo da solicitação, forneça uma representação JSON do objeto managedAndroidStoreApp.</span><span class="sxs-lookup"><span data-stu-id="8664e-128">In the request body, supply a JSON representation for the managedAndroidStoreApp object.</span></span>

<span data-ttu-id="8664e-129">A tabela a seguir mostra as propriedades obrigatórias ao criar managedAndroidStoreApp.</span><span class="sxs-lookup"><span data-stu-id="8664e-129">The following table shows the properties that are required when you create the managedAndroidStoreApp.</span></span>

|<span data-ttu-id="8664e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8664e-130">Property</span></span>|<span data-ttu-id="8664e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8664e-131">Type</span></span>|<span data-ttu-id="8664e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8664e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8664e-133">id</span><span class="sxs-lookup"><span data-stu-id="8664e-133">id</span></span>|<span data-ttu-id="8664e-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8664e-134">String</span></span>|<span data-ttu-id="8664e-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="8664e-135">Key of the entity.</span></span> <span data-ttu-id="8664e-136">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8664e-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8664e-137">displayName</span><span class="sxs-lookup"><span data-stu-id="8664e-137">displayName</span></span>|<span data-ttu-id="8664e-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8664e-138">String</span></span>|<span data-ttu-id="8664e-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="8664e-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="8664e-140">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8664e-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8664e-141">description</span><span class="sxs-lookup"><span data-stu-id="8664e-141">description</span></span>|<span data-ttu-id="8664e-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8664e-142">String</span></span>|<span data-ttu-id="8664e-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8664e-143">The description of the app.</span></span> <span data-ttu-id="8664e-144">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8664e-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8664e-145">publisher</span><span class="sxs-lookup"><span data-stu-id="8664e-145">publisher</span></span>|<span data-ttu-id="8664e-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8664e-146">String</span></span>|<span data-ttu-id="8664e-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8664e-147">The publisher of the app.</span></span> <span data-ttu-id="8664e-148">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8664e-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8664e-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="8664e-149">largeIcon</span></span>|[<span data-ttu-id="8664e-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="8664e-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="8664e-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="8664e-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="8664e-152">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8664e-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8664e-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8664e-153">createdDateTime</span></span>|<span data-ttu-id="8664e-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8664e-154">DateTimeOffset</span></span>|<span data-ttu-id="8664e-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8664e-155">The date and time the app was created.</span></span> <span data-ttu-id="8664e-156">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8664e-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8664e-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8664e-157">lastModifiedDateTime</span></span>|<span data-ttu-id="8664e-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8664e-158">DateTimeOffset</span></span>|<span data-ttu-id="8664e-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="8664e-159">The date and time the app was last modified.</span></span> <span data-ttu-id="8664e-160">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8664e-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8664e-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="8664e-161">isFeatured</span></span>|<span data-ttu-id="8664e-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="8664e-162">Boolean</span></span>|<span data-ttu-id="8664e-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8664e-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8664e-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="8664e-164">privacyInformationUrl</span></span>|<span data-ttu-id="8664e-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8664e-165">String</span></span>|<span data-ttu-id="8664e-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="8664e-166">The privacy statement Url.</span></span> <span data-ttu-id="8664e-167">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8664e-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8664e-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="8664e-168">informationUrl</span></span>|<span data-ttu-id="8664e-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8664e-169">String</span></span>|<span data-ttu-id="8664e-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="8664e-170">The more information Url.</span></span> <span data-ttu-id="8664e-171">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8664e-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8664e-172">owner</span><span class="sxs-lookup"><span data-stu-id="8664e-172">owner</span></span>|<span data-ttu-id="8664e-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8664e-173">String</span></span>|<span data-ttu-id="8664e-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="8664e-174">The owner of the app.</span></span> <span data-ttu-id="8664e-175">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8664e-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8664e-176">developer</span><span class="sxs-lookup"><span data-stu-id="8664e-176">developer</span></span>|<span data-ttu-id="8664e-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8664e-177">String</span></span>|<span data-ttu-id="8664e-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8664e-178">The developer of the app.</span></span> <span data-ttu-id="8664e-179">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8664e-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8664e-180">Observações</span><span class="sxs-lookup"><span data-stu-id="8664e-180">notes</span></span>|<span data-ttu-id="8664e-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8664e-181">String</span></span>|<span data-ttu-id="8664e-182">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8664e-182">Notes for the app.</span></span> <span data-ttu-id="8664e-183">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8664e-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8664e-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="8664e-184">uploadState</span></span>|<span data-ttu-id="8664e-185">Int32</span><span class="sxs-lookup"><span data-stu-id="8664e-185">Int32</span></span>|<span data-ttu-id="8664e-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="8664e-186">The upload state.</span></span> <span data-ttu-id="8664e-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8664e-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8664e-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="8664e-188">publishingState</span></span>|[<span data-ttu-id="8664e-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="8664e-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="8664e-190">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8664e-190">The publishing state for the app.</span></span> <span data-ttu-id="8664e-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="8664e-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="8664e-192">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8664e-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="8664e-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="8664e-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="8664e-194">appAvailability</span><span class="sxs-lookup"><span data-stu-id="8664e-194">appAvailability</span></span>|[<span data-ttu-id="8664e-195">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="8664e-195">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="8664e-196">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8664e-196">The Application's availability.</span></span> <span data-ttu-id="8664e-197">Herdada do [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="8664e-197">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="8664e-198">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="8664e-198">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="8664e-199">version</span><span class="sxs-lookup"><span data-stu-id="8664e-199">version</span></span>|<span data-ttu-id="8664e-200">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8664e-200">String</span></span>|<span data-ttu-id="8664e-201">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8664e-201">The Application's version.</span></span> <span data-ttu-id="8664e-202">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="8664e-202">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="8664e-203">packageId</span><span class="sxs-lookup"><span data-stu-id="8664e-203">packageId</span></span>|<span data-ttu-id="8664e-204">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8664e-204">String</span></span>|<span data-ttu-id="8664e-205">A ID de pacote do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8664e-205">The app's package ID.</span></span>|
|<span data-ttu-id="8664e-206">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="8664e-206">appStoreUrl</span></span>|<span data-ttu-id="8664e-207">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8664e-207">String</span></span>|<span data-ttu-id="8664e-208">A AppStoreUrl do Android.</span><span class="sxs-lookup"><span data-stu-id="8664e-208">The Android AppStoreUrl.</span></span>|
|<span data-ttu-id="8664e-209">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="8664e-209">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="8664e-210">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="8664e-210">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="8664e-211">O valor do sistema operacional mínimo com suporte.</span><span class="sxs-lookup"><span data-stu-id="8664e-211">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="8664e-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="8664e-212">Response</span></span>
<span data-ttu-id="8664e-213">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8664e-213">If successful, this method returns a `201 Created` response code and a [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8664e-214">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8664e-214">Example</span></span>
### <a name="request"></a><span data-ttu-id="8664e-215">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8664e-215">Request</span></span>
<span data-ttu-id="8664e-216">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8664e-216">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1216

{
  "@odata.type": "#microsoft.graph.managedAndroidStoreApp",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "packageId": "Package Id value",
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

### <a name="response"></a><span data-ttu-id="8664e-217">Resposta</span><span class="sxs-lookup"><span data-stu-id="8664e-217">Response</span></span>
<span data-ttu-id="8664e-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8664e-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1324

{
  "@odata.type": "#microsoft.graph.managedAndroidStoreApp",
  "id": "89e7e991-e991-89e7-91e9-e78991e9e789",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "packageId": "Package Id value",
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





