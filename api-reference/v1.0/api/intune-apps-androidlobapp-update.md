---
title: Atualizar androidLobApp
description: Atualiza as propriedades de um objeto androidLobApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e8fffc2d746be5bced923897808e924458bd8ce4
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30968375"
---
# <a name="update-androidlobapp"></a><span data-ttu-id="41adb-103">Atualizar androidLobApp</span><span class="sxs-lookup"><span data-stu-id="41adb-103">Update androidLobApp</span></span>

> <span data-ttu-id="41adb-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="41adb-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41adb-105">Atualiza as propriedades de um objeto [androidLobApp](../resources/intune-apps-androidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="41adb-105">Update the properties of a [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="41adb-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="41adb-106">Prerequisites</span></span>
<span data-ttu-id="41adb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41adb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41adb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="41adb-109">Permission type</span></span>|<span data-ttu-id="41adb-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="41adb-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41adb-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="41adb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="41adb-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41adb-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="41adb-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="41adb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41adb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="41adb-114">Not supported.</span></span>|
|<span data-ttu-id="41adb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="41adb-115">Application</span></span>|<span data-ttu-id="41adb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="41adb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="41adb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="41adb-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="41adb-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="41adb-118">Request headers</span></span>
|<span data-ttu-id="41adb-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="41adb-119">Header</span></span>|<span data-ttu-id="41adb-120">Valor</span><span class="sxs-lookup"><span data-stu-id="41adb-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41adb-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="41adb-121">Authorization</span></span>|<span data-ttu-id="41adb-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="41adb-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="41adb-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="41adb-123">Accept</span></span>|<span data-ttu-id="41adb-124">application/json</span><span class="sxs-lookup"><span data-stu-id="41adb-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41adb-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="41adb-125">Request body</span></span>
<span data-ttu-id="41adb-126">No corpo da solicitação, forneça uma representação JSON do objeto [androidLobApp](../resources/intune-apps-androidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="41adb-126">In the request body, supply a JSON representation for the [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>

<span data-ttu-id="41adb-127">A tabela a seguir mostra as propriedades obrigatórias ao criar [androidLobApp](../resources/intune-apps-androidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="41adb-127">The following table shows the properties that are required when you create the [androidLobApp](../resources/intune-apps-androidlobapp.md).</span></span>

|<span data-ttu-id="41adb-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="41adb-128">Property</span></span>|<span data-ttu-id="41adb-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="41adb-129">Type</span></span>|<span data-ttu-id="41adb-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="41adb-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41adb-131">id</span><span class="sxs-lookup"><span data-stu-id="41adb-131">id</span></span>|<span data-ttu-id="41adb-132">String</span><span class="sxs-lookup"><span data-stu-id="41adb-132">String</span></span>|<span data-ttu-id="41adb-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="41adb-133">Key of the entity.</span></span> <span data-ttu-id="41adb-134">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="41adb-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="41adb-135">displayName</span><span class="sxs-lookup"><span data-stu-id="41adb-135">displayName</span></span>|<span data-ttu-id="41adb-136">String</span><span class="sxs-lookup"><span data-stu-id="41adb-136">String</span></span>|<span data-ttu-id="41adb-137">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="41adb-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="41adb-138">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="41adb-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="41adb-139">descrição</span><span class="sxs-lookup"><span data-stu-id="41adb-139">description</span></span>|<span data-ttu-id="41adb-140">String</span><span class="sxs-lookup"><span data-stu-id="41adb-140">String</span></span>|<span data-ttu-id="41adb-141">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="41adb-141">The description of the app.</span></span> <span data-ttu-id="41adb-142">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="41adb-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="41adb-143">publicador</span><span class="sxs-lookup"><span data-stu-id="41adb-143">publisher</span></span>|<span data-ttu-id="41adb-144">String</span><span class="sxs-lookup"><span data-stu-id="41adb-144">String</span></span>|<span data-ttu-id="41adb-145">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="41adb-145">The publisher of the app.</span></span> <span data-ttu-id="41adb-146">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="41adb-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="41adb-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="41adb-147">largeIcon</span></span>|[<span data-ttu-id="41adb-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="41adb-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="41adb-149">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="41adb-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="41adb-150">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="41adb-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="41adb-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="41adb-151">createdDateTime</span></span>|<span data-ttu-id="41adb-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41adb-152">DateTimeOffset</span></span>|<span data-ttu-id="41adb-153">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="41adb-153">The date and time the app was created.</span></span> <span data-ttu-id="41adb-154">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="41adb-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="41adb-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="41adb-155">lastModifiedDateTime</span></span>|<span data-ttu-id="41adb-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41adb-156">DateTimeOffset</span></span>|<span data-ttu-id="41adb-157">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="41adb-157">The date and time the app was last modified.</span></span> <span data-ttu-id="41adb-158">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="41adb-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="41adb-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="41adb-159">isFeatured</span></span>|<span data-ttu-id="41adb-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="41adb-160">Boolean</span></span>|<span data-ttu-id="41adb-161">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="41adb-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="41adb-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="41adb-162">privacyInformationUrl</span></span>|<span data-ttu-id="41adb-163">String</span><span class="sxs-lookup"><span data-stu-id="41adb-163">String</span></span>|<span data-ttu-id="41adb-164">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="41adb-164">The privacy statement Url.</span></span> <span data-ttu-id="41adb-165">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="41adb-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="41adb-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="41adb-166">informationUrl</span></span>|<span data-ttu-id="41adb-167">String</span><span class="sxs-lookup"><span data-stu-id="41adb-167">String</span></span>|<span data-ttu-id="41adb-168">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="41adb-168">The more information Url.</span></span> <span data-ttu-id="41adb-169">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="41adb-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="41adb-170">owner</span><span class="sxs-lookup"><span data-stu-id="41adb-170">owner</span></span>|<span data-ttu-id="41adb-171">String</span><span class="sxs-lookup"><span data-stu-id="41adb-171">String</span></span>|<span data-ttu-id="41adb-172">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="41adb-172">The owner of the app.</span></span> <span data-ttu-id="41adb-173">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="41adb-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="41adb-174">developer</span><span class="sxs-lookup"><span data-stu-id="41adb-174">developer</span></span>|<span data-ttu-id="41adb-175">String</span><span class="sxs-lookup"><span data-stu-id="41adb-175">String</span></span>|<span data-ttu-id="41adb-176">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="41adb-176">The developer of the app.</span></span> <span data-ttu-id="41adb-177">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="41adb-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="41adb-178">notes</span><span class="sxs-lookup"><span data-stu-id="41adb-178">notes</span></span>|<span data-ttu-id="41adb-179">String</span><span class="sxs-lookup"><span data-stu-id="41adb-179">String</span></span>|<span data-ttu-id="41adb-180">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="41adb-180">Notes for the app.</span></span> <span data-ttu-id="41adb-181">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="41adb-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="41adb-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="41adb-182">publishingState</span></span>|[<span data-ttu-id="41adb-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="41adb-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="41adb-184">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="41adb-184">The publishing state for the app.</span></span> <span data-ttu-id="41adb-185">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="41adb-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="41adb-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="41adb-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="41adb-187">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="41adb-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="41adb-188">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="41adb-188">committedContentVersion</span></span>|<span data-ttu-id="41adb-189">String</span><span class="sxs-lookup"><span data-stu-id="41adb-189">String</span></span>|<span data-ttu-id="41adb-190">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="41adb-190">The internal committed content version.</span></span> <span data-ttu-id="41adb-191">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="41adb-191">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="41adb-192">fileName</span><span class="sxs-lookup"><span data-stu-id="41adb-192">fileName</span></span>|<span data-ttu-id="41adb-193">String</span><span class="sxs-lookup"><span data-stu-id="41adb-193">String</span></span>|<span data-ttu-id="41adb-194">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="41adb-194">The name of the main Lob application file.</span></span> <span data-ttu-id="41adb-195">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="41adb-195">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="41adb-196">size</span><span class="sxs-lookup"><span data-stu-id="41adb-196">size</span></span>|<span data-ttu-id="41adb-197">Int64</span><span class="sxs-lookup"><span data-stu-id="41adb-197">Int64</span></span>|<span data-ttu-id="41adb-198">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="41adb-198">The total size, including all uploaded files.</span></span> <span data-ttu-id="41adb-199">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="41adb-199">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="41adb-200">packageId</span><span class="sxs-lookup"><span data-stu-id="41adb-200">packageId</span></span>|<span data-ttu-id="41adb-201">String</span><span class="sxs-lookup"><span data-stu-id="41adb-201">String</span></span>|<span data-ttu-id="41adb-202">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="41adb-202">The package identifier.</span></span>|
|<span data-ttu-id="41adb-203">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="41adb-203">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="41adb-204">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="41adb-204">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="41adb-205">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="41adb-205">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="41adb-206">versionName</span><span class="sxs-lookup"><span data-stu-id="41adb-206">versionName</span></span>|<span data-ttu-id="41adb-207">String</span><span class="sxs-lookup"><span data-stu-id="41adb-207">String</span></span>|<span data-ttu-id="41adb-208">O nome da versão do aplicativo de Linha de Negócios (LoB) Android.</span><span class="sxs-lookup"><span data-stu-id="41adb-208">The version name of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="41adb-209">versionCode</span><span class="sxs-lookup"><span data-stu-id="41adb-209">versionCode</span></span>|<span data-ttu-id="41adb-210">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="41adb-210">String</span></span>|<span data-ttu-id="41adb-211">O código da versão do aplicativo de Linha de Negócios (LoB) Android.</span><span class="sxs-lookup"><span data-stu-id="41adb-211">The version code of Android Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="41adb-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="41adb-212">Response</span></span>
<span data-ttu-id="41adb-213">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [androidLobApp](../resources/intune-apps-androidlobapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="41adb-213">If successful, this method returns a `200 OK` response code and an updated [androidLobApp](../resources/intune-apps-androidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41adb-214">Exemplo</span><span class="sxs-lookup"><span data-stu-id="41adb-214">Example</span></span>

### <a name="request"></a><span data-ttu-id="41adb-215">Solicitação</span><span class="sxs-lookup"><span data-stu-id="41adb-215">Request</span></span>
<span data-ttu-id="41adb-216">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="41adb-216">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
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

### <a name="response"></a><span data-ttu-id="41adb-217">Resposta</span><span class="sxs-lookup"><span data-stu-id="41adb-217">Response</span></span>
<span data-ttu-id="41adb-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="41adb-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



