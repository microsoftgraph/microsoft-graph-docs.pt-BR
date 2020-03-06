---
title: Criar androidLobApp
description: Cria um novo objeto androidLobApp.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 908710b779a62d17749eec009ccf031f4f25bb7f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42516693"
---
# <a name="create-androidlobapp"></a><span data-ttu-id="71fd4-103">Criar androidLobApp</span><span class="sxs-lookup"><span data-stu-id="71fd4-103">Create androidLobApp</span></span>

<span data-ttu-id="71fd4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71fd4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="71fd4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="71fd4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71fd4-106">Cria um novo objeto [androidLobApp](../resources/intune-apps-androidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="71fd4-106">Create a new [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="71fd4-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="71fd4-107">Prerequisites</span></span>
<span data-ttu-id="71fd4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71fd4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71fd4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="71fd4-110">Permission type</span></span>|<span data-ttu-id="71fd4-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="71fd4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71fd4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="71fd4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="71fd4-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71fd4-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="71fd4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="71fd4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71fd4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="71fd4-115">Not supported.</span></span>|
|<span data-ttu-id="71fd4-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="71fd4-116">Application</span></span>|<span data-ttu-id="71fd4-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="71fd4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="71fd4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="71fd4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="71fd4-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="71fd4-119">Request headers</span></span>
|<span data-ttu-id="71fd4-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="71fd4-120">Header</span></span>|<span data-ttu-id="71fd4-121">Valor</span><span class="sxs-lookup"><span data-stu-id="71fd4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71fd4-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="71fd4-122">Authorization</span></span>|<span data-ttu-id="71fd4-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="71fd4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71fd4-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="71fd4-124">Accept</span></span>|<span data-ttu-id="71fd4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="71fd4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71fd4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="71fd4-126">Request body</span></span>
<span data-ttu-id="71fd4-127">No corpo da solicitação, forneça uma representação JSON do objeto androidLobApp.</span><span class="sxs-lookup"><span data-stu-id="71fd4-127">In the request body, supply a JSON representation for the androidLobApp object.</span></span>

<span data-ttu-id="71fd4-128">A tabela a seguir mostra as propriedades obrigatórias ao criar androidLobApp.</span><span class="sxs-lookup"><span data-stu-id="71fd4-128">The following table shows the properties that are required when you create the androidLobApp.</span></span>

|<span data-ttu-id="71fd4-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="71fd4-129">Property</span></span>|<span data-ttu-id="71fd4-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="71fd4-130">Type</span></span>|<span data-ttu-id="71fd4-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="71fd4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71fd4-132">id</span><span class="sxs-lookup"><span data-stu-id="71fd4-132">id</span></span>|<span data-ttu-id="71fd4-133">String</span><span class="sxs-lookup"><span data-stu-id="71fd4-133">String</span></span>|<span data-ttu-id="71fd4-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="71fd4-134">Key of the entity.</span></span> <span data-ttu-id="71fd4-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="71fd4-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71fd4-136">displayName</span><span class="sxs-lookup"><span data-stu-id="71fd4-136">displayName</span></span>|<span data-ttu-id="71fd4-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="71fd4-137">String</span></span>|<span data-ttu-id="71fd4-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="71fd4-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="71fd4-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="71fd4-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71fd4-140">description</span><span class="sxs-lookup"><span data-stu-id="71fd4-140">description</span></span>|<span data-ttu-id="71fd4-141">String</span><span class="sxs-lookup"><span data-stu-id="71fd4-141">String</span></span>|<span data-ttu-id="71fd4-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="71fd4-142">The description of the app.</span></span> <span data-ttu-id="71fd4-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="71fd4-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71fd4-144">publicador</span><span class="sxs-lookup"><span data-stu-id="71fd4-144">publisher</span></span>|<span data-ttu-id="71fd4-145">String</span><span class="sxs-lookup"><span data-stu-id="71fd4-145">String</span></span>|<span data-ttu-id="71fd4-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="71fd4-146">The publisher of the app.</span></span> <span data-ttu-id="71fd4-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="71fd4-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71fd4-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="71fd4-148">largeIcon</span></span>|[<span data-ttu-id="71fd4-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="71fd4-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="71fd4-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="71fd4-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="71fd4-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="71fd4-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71fd4-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="71fd4-152">createdDateTime</span></span>|<span data-ttu-id="71fd4-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71fd4-153">DateTimeOffset</span></span>|<span data-ttu-id="71fd4-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="71fd4-154">The date and time the app was created.</span></span> <span data-ttu-id="71fd4-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="71fd4-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71fd4-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="71fd4-156">lastModifiedDateTime</span></span>|<span data-ttu-id="71fd4-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71fd4-157">DateTimeOffset</span></span>|<span data-ttu-id="71fd4-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="71fd4-158">The date and time the app was last modified.</span></span> <span data-ttu-id="71fd4-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="71fd4-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71fd4-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="71fd4-160">isFeatured</span></span>|<span data-ttu-id="71fd4-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="71fd4-161">Boolean</span></span>|<span data-ttu-id="71fd4-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="71fd4-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71fd4-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="71fd4-163">privacyInformationUrl</span></span>|<span data-ttu-id="71fd4-164">String</span><span class="sxs-lookup"><span data-stu-id="71fd4-164">String</span></span>|<span data-ttu-id="71fd4-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="71fd4-165">The privacy statement Url.</span></span> <span data-ttu-id="71fd4-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="71fd4-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71fd4-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="71fd4-167">informationUrl</span></span>|<span data-ttu-id="71fd4-168">String</span><span class="sxs-lookup"><span data-stu-id="71fd4-168">String</span></span>|<span data-ttu-id="71fd4-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="71fd4-169">The more information Url.</span></span> <span data-ttu-id="71fd4-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="71fd4-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71fd4-171">owner</span><span class="sxs-lookup"><span data-stu-id="71fd4-171">owner</span></span>|<span data-ttu-id="71fd4-172">String</span><span class="sxs-lookup"><span data-stu-id="71fd4-172">String</span></span>|<span data-ttu-id="71fd4-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="71fd4-173">The owner of the app.</span></span> <span data-ttu-id="71fd4-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="71fd4-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71fd4-175">developer</span><span class="sxs-lookup"><span data-stu-id="71fd4-175">developer</span></span>|<span data-ttu-id="71fd4-176">String</span><span class="sxs-lookup"><span data-stu-id="71fd4-176">String</span></span>|<span data-ttu-id="71fd4-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="71fd4-177">The developer of the app.</span></span> <span data-ttu-id="71fd4-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="71fd4-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71fd4-179">notes</span><span class="sxs-lookup"><span data-stu-id="71fd4-179">notes</span></span>|<span data-ttu-id="71fd4-180">String</span><span class="sxs-lookup"><span data-stu-id="71fd4-180">String</span></span>|<span data-ttu-id="71fd4-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="71fd4-181">Notes for the app.</span></span> <span data-ttu-id="71fd4-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="71fd4-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="71fd4-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="71fd4-183">publishingState</span></span>|[<span data-ttu-id="71fd4-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="71fd4-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="71fd4-185">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="71fd4-185">The publishing state for the app.</span></span> <span data-ttu-id="71fd4-186">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="71fd4-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="71fd4-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="71fd4-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="71fd4-188">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="71fd4-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="71fd4-189">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="71fd4-189">committedContentVersion</span></span>|<span data-ttu-id="71fd4-190">String</span><span class="sxs-lookup"><span data-stu-id="71fd4-190">String</span></span>|<span data-ttu-id="71fd4-191">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="71fd4-191">The internal committed content version.</span></span> <span data-ttu-id="71fd4-192">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="71fd4-192">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="71fd4-193">fileName</span><span class="sxs-lookup"><span data-stu-id="71fd4-193">fileName</span></span>|<span data-ttu-id="71fd4-194">String</span><span class="sxs-lookup"><span data-stu-id="71fd4-194">String</span></span>|<span data-ttu-id="71fd4-195">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="71fd4-195">The name of the main Lob application file.</span></span> <span data-ttu-id="71fd4-196">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="71fd4-196">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="71fd4-197">size</span><span class="sxs-lookup"><span data-stu-id="71fd4-197">size</span></span>|<span data-ttu-id="71fd4-198">Int64</span><span class="sxs-lookup"><span data-stu-id="71fd4-198">Int64</span></span>|<span data-ttu-id="71fd4-199">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="71fd4-199">The total size, including all uploaded files.</span></span> <span data-ttu-id="71fd4-200">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="71fd4-200">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="71fd4-201">packageId</span><span class="sxs-lookup"><span data-stu-id="71fd4-201">packageId</span></span>|<span data-ttu-id="71fd4-202">String</span><span class="sxs-lookup"><span data-stu-id="71fd4-202">String</span></span>|<span data-ttu-id="71fd4-203">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="71fd4-203">The package identifier.</span></span>|
|<span data-ttu-id="71fd4-204">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="71fd4-204">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="71fd4-205">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="71fd4-205">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="71fd4-206">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="71fd4-206">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="71fd4-207">versionName</span><span class="sxs-lookup"><span data-stu-id="71fd4-207">versionName</span></span>|<span data-ttu-id="71fd4-208">String</span><span class="sxs-lookup"><span data-stu-id="71fd4-208">String</span></span>|<span data-ttu-id="71fd4-209">O nome da versão do aplicativo de Linha de Negócios (LoB) Android.</span><span class="sxs-lookup"><span data-stu-id="71fd4-209">The version name of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="71fd4-210">versionCode</span><span class="sxs-lookup"><span data-stu-id="71fd4-210">versionCode</span></span>|<span data-ttu-id="71fd4-211">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="71fd4-211">String</span></span>|<span data-ttu-id="71fd4-212">O código da versão do aplicativo de Linha de Negócios (LoB) Android.</span><span class="sxs-lookup"><span data-stu-id="71fd4-212">The version code of Android Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="71fd4-213">Resposta</span><span class="sxs-lookup"><span data-stu-id="71fd4-213">Response</span></span>
<span data-ttu-id="71fd4-214">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [androidLobApp](../resources/intune-apps-androidlobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="71fd4-214">If successful, this method returns a `201 Created` response code and a [androidLobApp](../resources/intune-apps-androidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71fd4-215">Exemplo</span><span class="sxs-lookup"><span data-stu-id="71fd4-215">Example</span></span>

### <a name="request"></a><span data-ttu-id="71fd4-216">Solicitação</span><span class="sxs-lookup"><span data-stu-id="71fd4-216">Request</span></span>
<span data-ttu-id="71fd4-217">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="71fd4-217">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1075

{
  "@odata.type": "#microsoft.graph.androidLobApp",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value"
}
```

### <a name="response"></a><span data-ttu-id="71fd4-218">Resposta</span><span class="sxs-lookup"><span data-stu-id="71fd4-218">Response</span></span>
<span data-ttu-id="71fd4-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="71fd4-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1247

{
  "@odata.type": "#microsoft.graph.androidLobApp",
  "id": "4b9a27d0-27d0-4b9a-d027-9a4bd0279a4b",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value"
}
```




