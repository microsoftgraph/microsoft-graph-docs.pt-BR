---
title: Criar windowsMobileMSI
description: Cria um novo objeto windowsMobileMSI.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8597dbe9e6526519b658c992f2aa2ef4fa27ab48
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48063531"
---
# <a name="create-windowsmobilemsi"></a><span data-ttu-id="108f3-103">Criar windowsMobileMSI</span><span class="sxs-lookup"><span data-stu-id="108f3-103">Create windowsMobileMSI</span></span>

<span data-ttu-id="108f3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="108f3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="108f3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="108f3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="108f3-106">Cria um novo objeto [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="108f3-106">Create a new [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="108f3-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="108f3-107">Prerequisites</span></span>
<span data-ttu-id="108f3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="108f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="108f3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="108f3-110">Permission type</span></span>|<span data-ttu-id="108f3-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="108f3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="108f3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="108f3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="108f3-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="108f3-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="108f3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="108f3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="108f3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="108f3-115">Not supported.</span></span>|
|<span data-ttu-id="108f3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="108f3-116">Application</span></span>|<span data-ttu-id="108f3-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="108f3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="108f3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="108f3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="108f3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="108f3-119">Request headers</span></span>
|<span data-ttu-id="108f3-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="108f3-120">Header</span></span>|<span data-ttu-id="108f3-121">Valor</span><span class="sxs-lookup"><span data-stu-id="108f3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="108f3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="108f3-122">Authorization</span></span>|<span data-ttu-id="108f3-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="108f3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="108f3-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="108f3-124">Accept</span></span>|<span data-ttu-id="108f3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="108f3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="108f3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="108f3-126">Request body</span></span>
<span data-ttu-id="108f3-127">No corpo da solicitação, forneça uma representação JSON para o objeto windowsMobileMSI.</span><span class="sxs-lookup"><span data-stu-id="108f3-127">In the request body, supply a JSON representation for the windowsMobileMSI object.</span></span>

<span data-ttu-id="108f3-128">A tabela a seguir mostra as propriedades obrigatórias ao criar windowsMobileMSI.</span><span class="sxs-lookup"><span data-stu-id="108f3-128">The following table shows the properties that are required when you create the windowsMobileMSI.</span></span>

|<span data-ttu-id="108f3-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="108f3-129">Property</span></span>|<span data-ttu-id="108f3-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="108f3-130">Type</span></span>|<span data-ttu-id="108f3-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="108f3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="108f3-132">id</span><span class="sxs-lookup"><span data-stu-id="108f3-132">id</span></span>|<span data-ttu-id="108f3-133">String</span><span class="sxs-lookup"><span data-stu-id="108f3-133">String</span></span>|<span data-ttu-id="108f3-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="108f3-134">Key of the entity.</span></span> <span data-ttu-id="108f3-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="108f3-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="108f3-136">displayName</span><span class="sxs-lookup"><span data-stu-id="108f3-136">displayName</span></span>|<span data-ttu-id="108f3-137">String</span><span class="sxs-lookup"><span data-stu-id="108f3-137">String</span></span>|<span data-ttu-id="108f3-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="108f3-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="108f3-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="108f3-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="108f3-140">description</span><span class="sxs-lookup"><span data-stu-id="108f3-140">description</span></span>|<span data-ttu-id="108f3-141">String</span><span class="sxs-lookup"><span data-stu-id="108f3-141">String</span></span>|<span data-ttu-id="108f3-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="108f3-142">The description of the app.</span></span> <span data-ttu-id="108f3-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="108f3-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="108f3-144">publicador</span><span class="sxs-lookup"><span data-stu-id="108f3-144">publisher</span></span>|<span data-ttu-id="108f3-145">String</span><span class="sxs-lookup"><span data-stu-id="108f3-145">String</span></span>|<span data-ttu-id="108f3-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="108f3-146">The publisher of the app.</span></span> <span data-ttu-id="108f3-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="108f3-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="108f3-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="108f3-148">largeIcon</span></span>|[<span data-ttu-id="108f3-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="108f3-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="108f3-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="108f3-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="108f3-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="108f3-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="108f3-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="108f3-152">createdDateTime</span></span>|<span data-ttu-id="108f3-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="108f3-153">DateTimeOffset</span></span>|<span data-ttu-id="108f3-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="108f3-154">The date and time the app was created.</span></span> <span data-ttu-id="108f3-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="108f3-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="108f3-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="108f3-156">lastModifiedDateTime</span></span>|<span data-ttu-id="108f3-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="108f3-157">DateTimeOffset</span></span>|<span data-ttu-id="108f3-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="108f3-158">The date and time the app was last modified.</span></span> <span data-ttu-id="108f3-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="108f3-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="108f3-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="108f3-160">isFeatured</span></span>|<span data-ttu-id="108f3-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="108f3-161">Boolean</span></span>|<span data-ttu-id="108f3-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="108f3-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="108f3-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="108f3-163">privacyInformationUrl</span></span>|<span data-ttu-id="108f3-164">String</span><span class="sxs-lookup"><span data-stu-id="108f3-164">String</span></span>|<span data-ttu-id="108f3-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="108f3-165">The privacy statement Url.</span></span> <span data-ttu-id="108f3-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="108f3-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="108f3-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="108f3-167">informationUrl</span></span>|<span data-ttu-id="108f3-168">String</span><span class="sxs-lookup"><span data-stu-id="108f3-168">String</span></span>|<span data-ttu-id="108f3-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="108f3-169">The more information Url.</span></span> <span data-ttu-id="108f3-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="108f3-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="108f3-171">proprietário</span><span class="sxs-lookup"><span data-stu-id="108f3-171">owner</span></span>|<span data-ttu-id="108f3-172">String</span><span class="sxs-lookup"><span data-stu-id="108f3-172">String</span></span>|<span data-ttu-id="108f3-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="108f3-173">The owner of the app.</span></span> <span data-ttu-id="108f3-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="108f3-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="108f3-175">developer</span><span class="sxs-lookup"><span data-stu-id="108f3-175">developer</span></span>|<span data-ttu-id="108f3-176">String</span><span class="sxs-lookup"><span data-stu-id="108f3-176">String</span></span>|<span data-ttu-id="108f3-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="108f3-177">The developer of the app.</span></span> <span data-ttu-id="108f3-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="108f3-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="108f3-179">notes</span><span class="sxs-lookup"><span data-stu-id="108f3-179">notes</span></span>|<span data-ttu-id="108f3-180">String</span><span class="sxs-lookup"><span data-stu-id="108f3-180">String</span></span>|<span data-ttu-id="108f3-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="108f3-181">Notes for the app.</span></span> <span data-ttu-id="108f3-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="108f3-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="108f3-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="108f3-183">publishingState</span></span>|[<span data-ttu-id="108f3-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="108f3-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="108f3-185">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="108f3-185">The publishing state for the app.</span></span> <span data-ttu-id="108f3-186">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="108f3-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="108f3-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="108f3-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="108f3-188">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="108f3-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="108f3-189">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="108f3-189">committedContentVersion</span></span>|<span data-ttu-id="108f3-190">String</span><span class="sxs-lookup"><span data-stu-id="108f3-190">String</span></span>|<span data-ttu-id="108f3-191">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="108f3-191">The internal committed content version.</span></span> <span data-ttu-id="108f3-192">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="108f3-192">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="108f3-193">fileName</span><span class="sxs-lookup"><span data-stu-id="108f3-193">fileName</span></span>|<span data-ttu-id="108f3-194">String</span><span class="sxs-lookup"><span data-stu-id="108f3-194">String</span></span>|<span data-ttu-id="108f3-195">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="108f3-195">The name of the main Lob application file.</span></span> <span data-ttu-id="108f3-196">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="108f3-196">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="108f3-197">size</span><span class="sxs-lookup"><span data-stu-id="108f3-197">size</span></span>|<span data-ttu-id="108f3-198">Int64</span><span class="sxs-lookup"><span data-stu-id="108f3-198">Int64</span></span>|<span data-ttu-id="108f3-199">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="108f3-199">The total size, including all uploaded files.</span></span> <span data-ttu-id="108f3-200">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="108f3-200">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="108f3-201">commandLine</span><span class="sxs-lookup"><span data-stu-id="108f3-201">commandLine</span></span>|<span data-ttu-id="108f3-202">String</span><span class="sxs-lookup"><span data-stu-id="108f3-202">String</span></span>|<span data-ttu-id="108f3-203">A linha de comando.</span><span class="sxs-lookup"><span data-stu-id="108f3-203">The command line.</span></span>|
|<span data-ttu-id="108f3-204">productCode</span><span class="sxs-lookup"><span data-stu-id="108f3-204">productCode</span></span>|<span data-ttu-id="108f3-205">String</span><span class="sxs-lookup"><span data-stu-id="108f3-205">String</span></span>|<span data-ttu-id="108f3-206">O código do produto.</span><span class="sxs-lookup"><span data-stu-id="108f3-206">The product code.</span></span>|
|<span data-ttu-id="108f3-207">productVersion</span><span class="sxs-lookup"><span data-stu-id="108f3-207">productVersion</span></span>|<span data-ttu-id="108f3-208">String</span><span class="sxs-lookup"><span data-stu-id="108f3-208">String</span></span>|<span data-ttu-id="108f3-209">A versão de produto do aplicativo de linha de negócios (LoB) Windows Mobile MSI.</span><span class="sxs-lookup"><span data-stu-id="108f3-209">The product version of Windows Mobile MSI Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="108f3-210">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="108f3-210">ignoreVersionDetection</span></span>|<span data-ttu-id="108f3-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="108f3-211">Boolean</span></span>|<span data-ttu-id="108f3-212">Um booliano para controlar se a versão do aplicativo será usada para detectar o aplicativo depois que ele for instalado em um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="108f3-212">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="108f3-213">Defina como true para o aplicativos de linha de negócios (LoB) Windows Mobile MSI que usam um recurso de atualização automática.</span><span class="sxs-lookup"><span data-stu-id="108f3-213">Set this to true for Windows Mobile MSI Line of Business (LoB) apps that use a self update feature.</span></span>|



## <a name="response"></a><span data-ttu-id="108f3-214">Resposta</span><span class="sxs-lookup"><span data-stu-id="108f3-214">Response</span></span>
<span data-ttu-id="108f3-215">Se tiver êxito, este método retornará o código de resposta `201 Created` e o objeto [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="108f3-215">If successful, this method returns a `201 Created` response code and a [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="108f3-216">Exemplo</span><span class="sxs-lookup"><span data-stu-id="108f3-216">Example</span></span>

### <a name="request"></a><span data-ttu-id="108f3-217">Solicitação</span><span class="sxs-lookup"><span data-stu-id="108f3-217">Request</span></span>
<span data-ttu-id="108f3-218">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="108f3-218">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="108f3-219">Resposta</span><span class="sxs-lookup"><span data-stu-id="108f3-219">Response</span></span>
<span data-ttu-id="108f3-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="108f3-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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









