---
title: Criar managedIOSStoreApp
description: Cria um novo objeto managedIOSStoreApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7f8d2748e3ea1c2b57a7e9906ae8d3bea11dcfec
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47997456"
---
# <a name="create-managediosstoreapp"></a><span data-ttu-id="f2b13-103">Criar managedIOSStoreApp</span><span class="sxs-lookup"><span data-stu-id="f2b13-103">Create managedIOSStoreApp</span></span>

<span data-ttu-id="f2b13-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2b13-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f2b13-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f2b13-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2b13-106">Cria um novo objeto [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="f2b13-106">Create a new [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f2b13-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f2b13-107">Prerequisites</span></span>
<span data-ttu-id="f2b13-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f2b13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f2b13-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f2b13-110">Permission type</span></span>|<span data-ttu-id="f2b13-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f2b13-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2b13-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f2b13-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f2b13-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2b13-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f2b13-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f2b13-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2b13-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f2b13-115">Not supported.</span></span>|
|<span data-ttu-id="f2b13-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f2b13-116">Application</span></span>|<span data-ttu-id="f2b13-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2b13-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2b13-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f2b13-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="f2b13-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f2b13-119">Request headers</span></span>
|<span data-ttu-id="f2b13-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f2b13-120">Header</span></span>|<span data-ttu-id="f2b13-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f2b13-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f2b13-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f2b13-122">Authorization</span></span>|<span data-ttu-id="f2b13-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f2b13-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f2b13-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f2b13-124">Accept</span></span>|<span data-ttu-id="f2b13-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f2b13-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2b13-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f2b13-126">Request body</span></span>
<span data-ttu-id="f2b13-127">No corpo da solicitação, forneça uma representação JSON do objeto managedIOSStoreApp.</span><span class="sxs-lookup"><span data-stu-id="f2b13-127">In the request body, supply a JSON representation for the managedIOSStoreApp object.</span></span>

<span data-ttu-id="f2b13-128">A tabela a seguir mostra as propriedades obrigatórias ao criar managedIOSStoreApp.</span><span class="sxs-lookup"><span data-stu-id="f2b13-128">The following table shows the properties that are required when you create the managedIOSStoreApp.</span></span>

|<span data-ttu-id="f2b13-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f2b13-129">Property</span></span>|<span data-ttu-id="f2b13-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2b13-130">Type</span></span>|<span data-ttu-id="f2b13-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2b13-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2b13-132">id</span><span class="sxs-lookup"><span data-stu-id="f2b13-132">id</span></span>|<span data-ttu-id="f2b13-133">String</span><span class="sxs-lookup"><span data-stu-id="f2b13-133">String</span></span>|<span data-ttu-id="f2b13-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f2b13-134">Key of the entity.</span></span> <span data-ttu-id="f2b13-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2b13-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f2b13-136">displayName</span><span class="sxs-lookup"><span data-stu-id="f2b13-136">displayName</span></span>|<span data-ttu-id="f2b13-137">String</span><span class="sxs-lookup"><span data-stu-id="f2b13-137">String</span></span>|<span data-ttu-id="f2b13-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="f2b13-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="f2b13-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2b13-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f2b13-140">description</span><span class="sxs-lookup"><span data-stu-id="f2b13-140">description</span></span>|<span data-ttu-id="f2b13-141">String</span><span class="sxs-lookup"><span data-stu-id="f2b13-141">String</span></span>|<span data-ttu-id="f2b13-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f2b13-142">The description of the app.</span></span> <span data-ttu-id="f2b13-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2b13-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f2b13-144">publicador</span><span class="sxs-lookup"><span data-stu-id="f2b13-144">publisher</span></span>|<span data-ttu-id="f2b13-145">String</span><span class="sxs-lookup"><span data-stu-id="f2b13-145">String</span></span>|<span data-ttu-id="f2b13-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f2b13-146">The publisher of the app.</span></span> <span data-ttu-id="f2b13-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2b13-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f2b13-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="f2b13-148">largeIcon</span></span>|[<span data-ttu-id="f2b13-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f2b13-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f2b13-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="f2b13-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="f2b13-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2b13-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f2b13-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f2b13-152">createdDateTime</span></span>|<span data-ttu-id="f2b13-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2b13-153">DateTimeOffset</span></span>|<span data-ttu-id="f2b13-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f2b13-154">The date and time the app was created.</span></span> <span data-ttu-id="f2b13-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2b13-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f2b13-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f2b13-156">lastModifiedDateTime</span></span>|<span data-ttu-id="f2b13-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2b13-157">DateTimeOffset</span></span>|<span data-ttu-id="f2b13-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="f2b13-158">The date and time the app was last modified.</span></span> <span data-ttu-id="f2b13-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2b13-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f2b13-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="f2b13-160">isFeatured</span></span>|<span data-ttu-id="f2b13-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="f2b13-161">Boolean</span></span>|<span data-ttu-id="f2b13-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2b13-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f2b13-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f2b13-163">privacyInformationUrl</span></span>|<span data-ttu-id="f2b13-164">String</span><span class="sxs-lookup"><span data-stu-id="f2b13-164">String</span></span>|<span data-ttu-id="f2b13-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="f2b13-165">The privacy statement Url.</span></span> <span data-ttu-id="f2b13-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2b13-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f2b13-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f2b13-167">informationUrl</span></span>|<span data-ttu-id="f2b13-168">String</span><span class="sxs-lookup"><span data-stu-id="f2b13-168">String</span></span>|<span data-ttu-id="f2b13-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="f2b13-169">The more information Url.</span></span> <span data-ttu-id="f2b13-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2b13-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f2b13-171">proprietário</span><span class="sxs-lookup"><span data-stu-id="f2b13-171">owner</span></span>|<span data-ttu-id="f2b13-172">String</span><span class="sxs-lookup"><span data-stu-id="f2b13-172">String</span></span>|<span data-ttu-id="f2b13-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="f2b13-173">The owner of the app.</span></span> <span data-ttu-id="f2b13-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2b13-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f2b13-175">developer</span><span class="sxs-lookup"><span data-stu-id="f2b13-175">developer</span></span>|<span data-ttu-id="f2b13-176">String</span><span class="sxs-lookup"><span data-stu-id="f2b13-176">String</span></span>|<span data-ttu-id="f2b13-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f2b13-177">The developer of the app.</span></span> <span data-ttu-id="f2b13-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2b13-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f2b13-179">notes</span><span class="sxs-lookup"><span data-stu-id="f2b13-179">notes</span></span>|<span data-ttu-id="f2b13-180">String</span><span class="sxs-lookup"><span data-stu-id="f2b13-180">String</span></span>|<span data-ttu-id="f2b13-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f2b13-181">Notes for the app.</span></span> <span data-ttu-id="f2b13-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2b13-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f2b13-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="f2b13-183">publishingState</span></span>|[<span data-ttu-id="f2b13-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="f2b13-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="f2b13-185">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f2b13-185">The publishing state for the app.</span></span> <span data-ttu-id="f2b13-186">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="f2b13-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="f2b13-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f2b13-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="f2b13-188">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="f2b13-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="f2b13-189">appAvailability</span><span class="sxs-lookup"><span data-stu-id="f2b13-189">appAvailability</span></span>|[<span data-ttu-id="f2b13-190">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="f2b13-190">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="f2b13-191">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f2b13-191">The Application's availability.</span></span> <span data-ttu-id="f2b13-192">Herdado de [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="f2b13-192">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="f2b13-193">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="f2b13-193">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="f2b13-194">version</span><span class="sxs-lookup"><span data-stu-id="f2b13-194">version</span></span>|<span data-ttu-id="f2b13-195">String</span><span class="sxs-lookup"><span data-stu-id="f2b13-195">String</span></span>|<span data-ttu-id="f2b13-196">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f2b13-196">The Application's version.</span></span> <span data-ttu-id="f2b13-197">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2b13-197">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="f2b13-198">bundleId</span><span class="sxs-lookup"><span data-stu-id="f2b13-198">bundleId</span></span>|<span data-ttu-id="f2b13-199">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2b13-199">String</span></span>|<span data-ttu-id="f2b13-200">A ID do pacote de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="f2b13-200">The app's Bundle ID.</span></span>|
|<span data-ttu-id="f2b13-201">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="f2b13-201">appStoreUrl</span></span>|<span data-ttu-id="f2b13-202">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2b13-202">String</span></span>|<span data-ttu-id="f2b13-203">A AppStoreUrl da Apple.</span><span class="sxs-lookup"><span data-stu-id="f2b13-203">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="f2b13-204">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="f2b13-204">applicableDeviceType</span></span>|[<span data-ttu-id="f2b13-205">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="f2b13-205">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="f2b13-206">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="f2b13-206">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="f2b13-207">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f2b13-207">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="f2b13-208">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f2b13-208">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="f2b13-209">O valor do sistema operacional mínimo com suporte.</span><span class="sxs-lookup"><span data-stu-id="f2b13-209">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="f2b13-210">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2b13-210">Response</span></span>
<span data-ttu-id="f2b13-211">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f2b13-211">If successful, this method returns a `201 Created` response code and a [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2b13-212">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f2b13-212">Example</span></span>

### <a name="request"></a><span data-ttu-id="f2b13-213">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f2b13-213">Request</span></span>
<span data-ttu-id="f2b13-214">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f2b13-214">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1104

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
    "v13_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="f2b13-215">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2b13-215">Response</span></span>
<span data-ttu-id="f2b13-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f2b13-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1276

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
    "v13_0": true
  }
}
```









