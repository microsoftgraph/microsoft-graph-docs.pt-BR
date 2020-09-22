---
title: Atualizar windowsMobileMSI
description: Atualiza as propriedades de um objeto windowsMobileMSI.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 72cc707aea4fb9c85ef8e9aae3914f4da69e4ab3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48063482"
---
# <a name="update-windowsmobilemsi"></a><span data-ttu-id="bf969-103">Atualizar windowsMobileMSI</span><span class="sxs-lookup"><span data-stu-id="bf969-103">Update windowsMobileMSI</span></span>

<span data-ttu-id="bf969-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf969-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bf969-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bf969-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf969-106">Atualiza as propriedades de um objeto [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="bf969-106">Update the properties of a [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bf969-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bf969-107">Prerequisites</span></span>
<span data-ttu-id="bf969-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf969-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf969-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bf969-110">Permission type</span></span>|<span data-ttu-id="bf969-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bf969-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bf969-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bf969-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bf969-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf969-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bf969-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bf969-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bf969-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bf969-115">Not supported.</span></span>|
|<span data-ttu-id="bf969-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bf969-116">Application</span></span>|<span data-ttu-id="bf969-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bf969-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bf969-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bf969-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="bf969-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bf969-119">Request headers</span></span>
|<span data-ttu-id="bf969-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bf969-120">Header</span></span>|<span data-ttu-id="bf969-121">Valor</span><span class="sxs-lookup"><span data-stu-id="bf969-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bf969-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="bf969-122">Authorization</span></span>|<span data-ttu-id="bf969-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bf969-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bf969-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bf969-124">Accept</span></span>|<span data-ttu-id="bf969-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bf969-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf969-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bf969-126">Request body</span></span>
<span data-ttu-id="bf969-127">No corpo da solicitação, forneça uma representação JSON para o objeto [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="bf969-127">In the request body, supply a JSON representation for the [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>

<span data-ttu-id="bf969-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="bf969-128">The following table shows the properties that are required when you create the [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span></span>

|<span data-ttu-id="bf969-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bf969-129">Property</span></span>|<span data-ttu-id="bf969-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="bf969-130">Type</span></span>|<span data-ttu-id="bf969-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="bf969-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf969-132">id</span><span class="sxs-lookup"><span data-stu-id="bf969-132">id</span></span>|<span data-ttu-id="bf969-133">String</span><span class="sxs-lookup"><span data-stu-id="bf969-133">String</span></span>|<span data-ttu-id="bf969-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="bf969-134">Key of the entity.</span></span> <span data-ttu-id="bf969-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bf969-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bf969-136">displayName</span><span class="sxs-lookup"><span data-stu-id="bf969-136">displayName</span></span>|<span data-ttu-id="bf969-137">String</span><span class="sxs-lookup"><span data-stu-id="bf969-137">String</span></span>|<span data-ttu-id="bf969-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="bf969-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="bf969-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bf969-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bf969-140">description</span><span class="sxs-lookup"><span data-stu-id="bf969-140">description</span></span>|<span data-ttu-id="bf969-141">String</span><span class="sxs-lookup"><span data-stu-id="bf969-141">String</span></span>|<span data-ttu-id="bf969-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bf969-142">The description of the app.</span></span> <span data-ttu-id="bf969-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bf969-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bf969-144">publicador</span><span class="sxs-lookup"><span data-stu-id="bf969-144">publisher</span></span>|<span data-ttu-id="bf969-145">String</span><span class="sxs-lookup"><span data-stu-id="bf969-145">String</span></span>|<span data-ttu-id="bf969-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bf969-146">The publisher of the app.</span></span> <span data-ttu-id="bf969-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bf969-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bf969-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="bf969-148">largeIcon</span></span>|[<span data-ttu-id="bf969-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="bf969-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="bf969-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="bf969-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="bf969-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bf969-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bf969-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bf969-152">createdDateTime</span></span>|<span data-ttu-id="bf969-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bf969-153">DateTimeOffset</span></span>|<span data-ttu-id="bf969-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bf969-154">The date and time the app was created.</span></span> <span data-ttu-id="bf969-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bf969-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bf969-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bf969-156">lastModifiedDateTime</span></span>|<span data-ttu-id="bf969-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bf969-157">DateTimeOffset</span></span>|<span data-ttu-id="bf969-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="bf969-158">The date and time the app was last modified.</span></span> <span data-ttu-id="bf969-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bf969-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bf969-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="bf969-160">isFeatured</span></span>|<span data-ttu-id="bf969-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf969-161">Boolean</span></span>|<span data-ttu-id="bf969-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bf969-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bf969-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="bf969-163">privacyInformationUrl</span></span>|<span data-ttu-id="bf969-164">String</span><span class="sxs-lookup"><span data-stu-id="bf969-164">String</span></span>|<span data-ttu-id="bf969-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="bf969-165">The privacy statement Url.</span></span> <span data-ttu-id="bf969-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bf969-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bf969-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="bf969-167">informationUrl</span></span>|<span data-ttu-id="bf969-168">String</span><span class="sxs-lookup"><span data-stu-id="bf969-168">String</span></span>|<span data-ttu-id="bf969-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="bf969-169">The more information Url.</span></span> <span data-ttu-id="bf969-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bf969-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bf969-171">proprietário</span><span class="sxs-lookup"><span data-stu-id="bf969-171">owner</span></span>|<span data-ttu-id="bf969-172">String</span><span class="sxs-lookup"><span data-stu-id="bf969-172">String</span></span>|<span data-ttu-id="bf969-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="bf969-173">The owner of the app.</span></span> <span data-ttu-id="bf969-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bf969-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bf969-175">developer</span><span class="sxs-lookup"><span data-stu-id="bf969-175">developer</span></span>|<span data-ttu-id="bf969-176">String</span><span class="sxs-lookup"><span data-stu-id="bf969-176">String</span></span>|<span data-ttu-id="bf969-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bf969-177">The developer of the app.</span></span> <span data-ttu-id="bf969-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bf969-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bf969-179">notes</span><span class="sxs-lookup"><span data-stu-id="bf969-179">notes</span></span>|<span data-ttu-id="bf969-180">String</span><span class="sxs-lookup"><span data-stu-id="bf969-180">String</span></span>|<span data-ttu-id="bf969-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bf969-181">Notes for the app.</span></span> <span data-ttu-id="bf969-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bf969-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bf969-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="bf969-183">publishingState</span></span>|[<span data-ttu-id="bf969-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="bf969-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="bf969-185">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bf969-185">The publishing state for the app.</span></span> <span data-ttu-id="bf969-186">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="bf969-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="bf969-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bf969-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="bf969-188">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="bf969-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="bf969-189">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="bf969-189">committedContentVersion</span></span>|<span data-ttu-id="bf969-190">String</span><span class="sxs-lookup"><span data-stu-id="bf969-190">String</span></span>|<span data-ttu-id="bf969-191">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="bf969-191">The internal committed content version.</span></span> <span data-ttu-id="bf969-192">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="bf969-192">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="bf969-193">fileName</span><span class="sxs-lookup"><span data-stu-id="bf969-193">fileName</span></span>|<span data-ttu-id="bf969-194">String</span><span class="sxs-lookup"><span data-stu-id="bf969-194">String</span></span>|<span data-ttu-id="bf969-195">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="bf969-195">The name of the main Lob application file.</span></span> <span data-ttu-id="bf969-196">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="bf969-196">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="bf969-197">size</span><span class="sxs-lookup"><span data-stu-id="bf969-197">size</span></span>|<span data-ttu-id="bf969-198">Int64</span><span class="sxs-lookup"><span data-stu-id="bf969-198">Int64</span></span>|<span data-ttu-id="bf969-199">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="bf969-199">The total size, including all uploaded files.</span></span> <span data-ttu-id="bf969-200">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="bf969-200">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="bf969-201">commandLine</span><span class="sxs-lookup"><span data-stu-id="bf969-201">commandLine</span></span>|<span data-ttu-id="bf969-202">String</span><span class="sxs-lookup"><span data-stu-id="bf969-202">String</span></span>|<span data-ttu-id="bf969-203">A linha de comando.</span><span class="sxs-lookup"><span data-stu-id="bf969-203">The command line.</span></span>|
|<span data-ttu-id="bf969-204">productCode</span><span class="sxs-lookup"><span data-stu-id="bf969-204">productCode</span></span>|<span data-ttu-id="bf969-205">String</span><span class="sxs-lookup"><span data-stu-id="bf969-205">String</span></span>|<span data-ttu-id="bf969-206">O código do produto.</span><span class="sxs-lookup"><span data-stu-id="bf969-206">The product code.</span></span>|
|<span data-ttu-id="bf969-207">productVersion</span><span class="sxs-lookup"><span data-stu-id="bf969-207">productVersion</span></span>|<span data-ttu-id="bf969-208">String</span><span class="sxs-lookup"><span data-stu-id="bf969-208">String</span></span>|<span data-ttu-id="bf969-209">A versão de produto do aplicativo de linha de negócios (LoB) Windows Mobile MSI.</span><span class="sxs-lookup"><span data-stu-id="bf969-209">The product version of Windows Mobile MSI Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="bf969-210">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="bf969-210">ignoreVersionDetection</span></span>|<span data-ttu-id="bf969-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf969-211">Boolean</span></span>|<span data-ttu-id="bf969-212">Um booliano para controlar se a versão do aplicativo será usada para detectar o aplicativo depois que ele for instalado em um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bf969-212">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="bf969-213">Defina como true para o aplicativos de linha de negócios (LoB) Windows Mobile MSI que usam um recurso de atualização automática.</span><span class="sxs-lookup"><span data-stu-id="bf969-213">Set this to true for Windows Mobile MSI Line of Business (LoB) apps that use a self update feature.</span></span>|



## <a name="response"></a><span data-ttu-id="bf969-214">Resposta</span><span class="sxs-lookup"><span data-stu-id="bf969-214">Response</span></span>
<span data-ttu-id="bf969-215">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bf969-215">If successful, this method returns a `200 OK` response code and an updated [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf969-216">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bf969-216">Example</span></span>

### <a name="request"></a><span data-ttu-id="bf969-217">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bf969-217">Request</span></span>
<span data-ttu-id="bf969-218">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bf969-218">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 855

{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
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
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true
}
```

### <a name="response"></a><span data-ttu-id="bf969-219">Resposta</span><span class="sxs-lookup"><span data-stu-id="bf969-219">Response</span></span>
<span data-ttu-id="bf969-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bf969-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1027

{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
  "id": "aa453e5d-3e5d-aa45-5d3e-45aa5d3e45aa",
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
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true
}
```









