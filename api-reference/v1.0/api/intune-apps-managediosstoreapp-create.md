---
title: Criar managedIOSStoreApp
description: Cria um novo objeto managedIOSStoreApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bde2728f147c7a7208156fede8ccc4722d3c8db0
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754172"
---
# <a name="create-managediosstoreapp"></a><span data-ttu-id="6db4b-103">Criar managedIOSStoreApp</span><span class="sxs-lookup"><span data-stu-id="6db4b-103">Create managedIOSStoreApp</span></span>

<span data-ttu-id="6db4b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6db4b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6db4b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6db4b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6db4b-106">Cria um novo objeto [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="6db4b-106">Create a new [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6db4b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6db4b-107">Prerequisites</span></span>
<span data-ttu-id="6db4b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6db4b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6db4b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6db4b-110">Permission type</span></span>|<span data-ttu-id="6db4b-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6db4b-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6db4b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6db4b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6db4b-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6db4b-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6db4b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6db4b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6db4b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6db4b-115">Not supported.</span></span>|
|<span data-ttu-id="6db4b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6db4b-116">Application</span></span>|<span data-ttu-id="6db4b-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6db4b-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6db4b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6db4b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="6db4b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6db4b-119">Request headers</span></span>
|<span data-ttu-id="6db4b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6db4b-120">Header</span></span>|<span data-ttu-id="6db4b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6db4b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6db4b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6db4b-122">Authorization</span></span>|<span data-ttu-id="6db4b-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6db4b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6db4b-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6db4b-124">Accept</span></span>|<span data-ttu-id="6db4b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6db4b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6db4b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6db4b-126">Request body</span></span>
<span data-ttu-id="6db4b-127">No corpo da solicitação, forneça uma representação JSON do objeto managedIOSStoreApp.</span><span class="sxs-lookup"><span data-stu-id="6db4b-127">In the request body, supply a JSON representation for the managedIOSStoreApp object.</span></span>

<span data-ttu-id="6db4b-128">A tabela a seguir mostra as propriedades obrigatórias ao criar managedIOSStoreApp.</span><span class="sxs-lookup"><span data-stu-id="6db4b-128">The following table shows the properties that are required when you create the managedIOSStoreApp.</span></span>

|<span data-ttu-id="6db4b-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6db4b-129">Property</span></span>|<span data-ttu-id="6db4b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="6db4b-130">Type</span></span>|<span data-ttu-id="6db4b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="6db4b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6db4b-132">id</span><span class="sxs-lookup"><span data-stu-id="6db4b-132">id</span></span>|<span data-ttu-id="6db4b-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6db4b-133">String</span></span>|<span data-ttu-id="6db4b-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6db4b-134">Key of the entity.</span></span> <span data-ttu-id="6db4b-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6db4b-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6db4b-136">displayName</span><span class="sxs-lookup"><span data-stu-id="6db4b-136">displayName</span></span>|<span data-ttu-id="6db4b-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6db4b-137">String</span></span>|<span data-ttu-id="6db4b-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="6db4b-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="6db4b-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6db4b-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6db4b-140">descrição</span><span class="sxs-lookup"><span data-stu-id="6db4b-140">description</span></span>|<span data-ttu-id="6db4b-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6db4b-141">String</span></span>|<span data-ttu-id="6db4b-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6db4b-142">The description of the app.</span></span> <span data-ttu-id="6db4b-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6db4b-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6db4b-144">publicador</span><span class="sxs-lookup"><span data-stu-id="6db4b-144">publisher</span></span>|<span data-ttu-id="6db4b-145">String</span><span class="sxs-lookup"><span data-stu-id="6db4b-145">String</span></span>|<span data-ttu-id="6db4b-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6db4b-146">The publisher of the app.</span></span> <span data-ttu-id="6db4b-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6db4b-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6db4b-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="6db4b-148">largeIcon</span></span>|[<span data-ttu-id="6db4b-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="6db4b-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="6db4b-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="6db4b-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="6db4b-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6db4b-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6db4b-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6db4b-152">createdDateTime</span></span>|<span data-ttu-id="6db4b-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6db4b-153">DateTimeOffset</span></span>|<span data-ttu-id="6db4b-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6db4b-154">The date and time the app was created.</span></span> <span data-ttu-id="6db4b-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6db4b-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6db4b-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6db4b-156">lastModifiedDateTime</span></span>|<span data-ttu-id="6db4b-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6db4b-157">DateTimeOffset</span></span>|<span data-ttu-id="6db4b-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="6db4b-158">The date and time the app was last modified.</span></span> <span data-ttu-id="6db4b-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6db4b-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6db4b-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="6db4b-160">isFeatured</span></span>|<span data-ttu-id="6db4b-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="6db4b-161">Boolean</span></span>|<span data-ttu-id="6db4b-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6db4b-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6db4b-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="6db4b-163">privacyInformationUrl</span></span>|<span data-ttu-id="6db4b-164">String</span><span class="sxs-lookup"><span data-stu-id="6db4b-164">String</span></span>|<span data-ttu-id="6db4b-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="6db4b-165">The privacy statement Url.</span></span> <span data-ttu-id="6db4b-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6db4b-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6db4b-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="6db4b-167">informationUrl</span></span>|<span data-ttu-id="6db4b-168">String</span><span class="sxs-lookup"><span data-stu-id="6db4b-168">String</span></span>|<span data-ttu-id="6db4b-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="6db4b-169">The more information Url.</span></span> <span data-ttu-id="6db4b-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6db4b-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6db4b-171">proprietário</span><span class="sxs-lookup"><span data-stu-id="6db4b-171">owner</span></span>|<span data-ttu-id="6db4b-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6db4b-172">String</span></span>|<span data-ttu-id="6db4b-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="6db4b-173">The owner of the app.</span></span> <span data-ttu-id="6db4b-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6db4b-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6db4b-175">developer</span><span class="sxs-lookup"><span data-stu-id="6db4b-175">developer</span></span>|<span data-ttu-id="6db4b-176">String</span><span class="sxs-lookup"><span data-stu-id="6db4b-176">String</span></span>|<span data-ttu-id="6db4b-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6db4b-177">The developer of the app.</span></span> <span data-ttu-id="6db4b-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6db4b-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6db4b-179">notes</span><span class="sxs-lookup"><span data-stu-id="6db4b-179">notes</span></span>|<span data-ttu-id="6db4b-180">String</span><span class="sxs-lookup"><span data-stu-id="6db4b-180">String</span></span>|<span data-ttu-id="6db4b-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6db4b-181">Notes for the app.</span></span> <span data-ttu-id="6db4b-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6db4b-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6db4b-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="6db4b-183">publishingState</span></span>|[<span data-ttu-id="6db4b-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="6db4b-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="6db4b-185">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6db4b-185">The publishing state for the app.</span></span> <span data-ttu-id="6db4b-186">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="6db4b-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="6db4b-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6db4b-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="6db4b-188">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="6db4b-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="6db4b-189">appAvailability</span><span class="sxs-lookup"><span data-stu-id="6db4b-189">appAvailability</span></span>|[<span data-ttu-id="6db4b-190">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="6db4b-190">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="6db4b-191">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6db4b-191">The Application's availability.</span></span> <span data-ttu-id="6db4b-192">Herdado [de managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="6db4b-192">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="6db4b-193">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="6db4b-193">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="6db4b-194">version</span><span class="sxs-lookup"><span data-stu-id="6db4b-194">version</span></span>|<span data-ttu-id="6db4b-195">String</span><span class="sxs-lookup"><span data-stu-id="6db4b-195">String</span></span>|<span data-ttu-id="6db4b-196">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6db4b-196">The Application's version.</span></span> <span data-ttu-id="6db4b-197">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="6db4b-197">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="6db4b-198">bundleId</span><span class="sxs-lookup"><span data-stu-id="6db4b-198">bundleId</span></span>|<span data-ttu-id="6db4b-199">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6db4b-199">String</span></span>|<span data-ttu-id="6db4b-200">A ID do pacote de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="6db4b-200">The app's Bundle ID.</span></span>|
|<span data-ttu-id="6db4b-201">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="6db4b-201">appStoreUrl</span></span>|<span data-ttu-id="6db4b-202">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6db4b-202">String</span></span>|<span data-ttu-id="6db4b-203">A AppStoreUrl da Apple.</span><span class="sxs-lookup"><span data-stu-id="6db4b-203">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="6db4b-204">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="6db4b-204">applicableDeviceType</span></span>|[<span data-ttu-id="6db4b-205">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="6db4b-205">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="6db4b-206">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="6db4b-206">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="6db4b-207">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="6db4b-207">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="6db4b-208">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="6db4b-208">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="6db4b-209">O valor do sistema operacional mínimo com suporte.</span><span class="sxs-lookup"><span data-stu-id="6db4b-209">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="6db4b-210">Resposta</span><span class="sxs-lookup"><span data-stu-id="6db4b-210">Response</span></span>
<span data-ttu-id="6db4b-211">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6db4b-211">If successful, this method returns a `201 Created` response code and a [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6db4b-212">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6db4b-212">Example</span></span>

### <a name="request"></a><span data-ttu-id="6db4b-213">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6db4b-213">Request</span></span>
<span data-ttu-id="6db4b-214">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6db4b-214">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1124

{
  "@odata.type": "#microsoft.graph.managedIOSStoreApp",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
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

### <a name="response"></a><span data-ttu-id="6db4b-215">Resposta</span><span class="sxs-lookup"><span data-stu-id="6db4b-215">Response</span></span>
<span data-ttu-id="6db4b-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6db4b-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1296

{
  "@odata.type": "#microsoft.graph.managedIOSStoreApp",
  "id": "51b9830f-830f-51b9-0f83-b9510f83b951",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
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




