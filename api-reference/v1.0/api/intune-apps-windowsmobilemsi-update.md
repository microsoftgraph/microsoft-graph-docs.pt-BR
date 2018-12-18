---
title: Atualizar windowsMobileMSI
description: Atualiza as propriedades de um objeto windowsMobileMSI.
author: tfitzmac
ms.openlocfilehash: eec168cff06f1ffbb2a78b0e2dd9151da04ff264
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27339295"
---
# <a name="update-windowsmobilemsi"></a><span data-ttu-id="34edb-103">Atualizar windowsMobileMSI</span><span class="sxs-lookup"><span data-stu-id="34edb-103">Update windowsMobileMSI</span></span>

> <span data-ttu-id="34edb-104">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="34edb-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="34edb-105">Atualiza as propriedades de um objeto [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="34edb-105">Update the properties of a [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="34edb-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="34edb-106">Prerequisites</span></span>
<span data-ttu-id="34edb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34edb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34edb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="34edb-109">Permission type</span></span>|<span data-ttu-id="34edb-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="34edb-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="34edb-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="34edb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="34edb-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34edb-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="34edb-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="34edb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="34edb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="34edb-114">Not supported.</span></span>|
|<span data-ttu-id="34edb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="34edb-115">Application</span></span>|<span data-ttu-id="34edb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="34edb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="34edb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="34edb-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="34edb-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="34edb-118">Request headers</span></span>
|<span data-ttu-id="34edb-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="34edb-119">Header</span></span>|<span data-ttu-id="34edb-120">Valor</span><span class="sxs-lookup"><span data-stu-id="34edb-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="34edb-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="34edb-121">Authorization</span></span>|<span data-ttu-id="34edb-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="34edb-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="34edb-123">Accept</span><span class="sxs-lookup"><span data-stu-id="34edb-123">Accept</span></span>|<span data-ttu-id="34edb-124">application/json</span><span class="sxs-lookup"><span data-stu-id="34edb-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="34edb-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="34edb-125">Request body</span></span>
<span data-ttu-id="34edb-126">No corpo da solicitação, forneça uma representação JSON para o objeto [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="34edb-126">In the request body, supply a JSON representation for the [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>

<span data-ttu-id="34edb-127">A tabela a seguir mostra as propriedades obrigatórias ao criar [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="34edb-127">The following table shows the properties that are required when you create the [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span></span>

|<span data-ttu-id="34edb-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="34edb-128">Property</span></span>|<span data-ttu-id="34edb-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="34edb-129">Type</span></span>|<span data-ttu-id="34edb-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="34edb-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34edb-131">id</span><span class="sxs-lookup"><span data-stu-id="34edb-131">id</span></span>|<span data-ttu-id="34edb-132">String</span><span class="sxs-lookup"><span data-stu-id="34edb-132">String</span></span>|<span data-ttu-id="34edb-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="34edb-133">Key of the entity.</span></span> <span data-ttu-id="34edb-134">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="34edb-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="34edb-135">displayName</span><span class="sxs-lookup"><span data-stu-id="34edb-135">displayName</span></span>|<span data-ttu-id="34edb-136">String</span><span class="sxs-lookup"><span data-stu-id="34edb-136">String</span></span>|<span data-ttu-id="34edb-137">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="34edb-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="34edb-138">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="34edb-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="34edb-139">description</span><span class="sxs-lookup"><span data-stu-id="34edb-139">description</span></span>|<span data-ttu-id="34edb-140">String</span><span class="sxs-lookup"><span data-stu-id="34edb-140">String</span></span>|<span data-ttu-id="34edb-141">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="34edb-141">The description of the app.</span></span> <span data-ttu-id="34edb-142">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="34edb-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="34edb-143">publisher</span><span class="sxs-lookup"><span data-stu-id="34edb-143">publisher</span></span>|<span data-ttu-id="34edb-144">String</span><span class="sxs-lookup"><span data-stu-id="34edb-144">String</span></span>|<span data-ttu-id="34edb-145">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="34edb-145">The publisher of the app.</span></span> <span data-ttu-id="34edb-146">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="34edb-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="34edb-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="34edb-147">largeIcon</span></span>|[<span data-ttu-id="34edb-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="34edb-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="34edb-149">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="34edb-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="34edb-150">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="34edb-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="34edb-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="34edb-151">createdDateTime</span></span>|<span data-ttu-id="34edb-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34edb-152">DateTimeOffset</span></span>|<span data-ttu-id="34edb-153">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="34edb-153">The date and time the app was created.</span></span> <span data-ttu-id="34edb-154">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="34edb-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="34edb-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="34edb-155">lastModifiedDateTime</span></span>|<span data-ttu-id="34edb-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34edb-156">DateTimeOffset</span></span>|<span data-ttu-id="34edb-157">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="34edb-157">The date and time the app was last modified.</span></span> <span data-ttu-id="34edb-158">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="34edb-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="34edb-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="34edb-159">isFeatured</span></span>|<span data-ttu-id="34edb-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="34edb-160">Boolean</span></span>|<span data-ttu-id="34edb-161">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="34edb-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="34edb-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="34edb-162">privacyInformationUrl</span></span>|<span data-ttu-id="34edb-163">String</span><span class="sxs-lookup"><span data-stu-id="34edb-163">String</span></span>|<span data-ttu-id="34edb-164">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="34edb-164">The privacy statement Url.</span></span> <span data-ttu-id="34edb-165">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="34edb-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="34edb-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="34edb-166">informationUrl</span></span>|<span data-ttu-id="34edb-167">String</span><span class="sxs-lookup"><span data-stu-id="34edb-167">String</span></span>|<span data-ttu-id="34edb-168">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="34edb-168">The more information Url.</span></span> <span data-ttu-id="34edb-169">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="34edb-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="34edb-170">owner</span><span class="sxs-lookup"><span data-stu-id="34edb-170">owner</span></span>|<span data-ttu-id="34edb-171">String</span><span class="sxs-lookup"><span data-stu-id="34edb-171">String</span></span>|<span data-ttu-id="34edb-172">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="34edb-172">The owner of the app.</span></span> <span data-ttu-id="34edb-173">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="34edb-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="34edb-174">developer</span><span class="sxs-lookup"><span data-stu-id="34edb-174">developer</span></span>|<span data-ttu-id="34edb-175">String</span><span class="sxs-lookup"><span data-stu-id="34edb-175">String</span></span>|<span data-ttu-id="34edb-176">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="34edb-176">The developer of the app.</span></span> <span data-ttu-id="34edb-177">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="34edb-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="34edb-178">Observações</span><span class="sxs-lookup"><span data-stu-id="34edb-178">notes</span></span>|<span data-ttu-id="34edb-179">String</span><span class="sxs-lookup"><span data-stu-id="34edb-179">String</span></span>|<span data-ttu-id="34edb-180">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="34edb-180">Notes for the app.</span></span> <span data-ttu-id="34edb-181">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="34edb-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="34edb-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="34edb-182">publishingState</span></span>|[<span data-ttu-id="34edb-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="34edb-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="34edb-184">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="34edb-184">The publishing state for the app.</span></span> <span data-ttu-id="34edb-185">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="34edb-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="34edb-186">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="34edb-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="34edb-187">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="34edb-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="34edb-188">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="34edb-188">committedContentVersion</span></span>|<span data-ttu-id="34edb-189">String</span><span class="sxs-lookup"><span data-stu-id="34edb-189">String</span></span>|<span data-ttu-id="34edb-190">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="34edb-190">The internal committed content version.</span></span> <span data-ttu-id="34edb-191">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="34edb-191">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="34edb-192">fileName</span><span class="sxs-lookup"><span data-stu-id="34edb-192">fileName</span></span>|<span data-ttu-id="34edb-193">String</span><span class="sxs-lookup"><span data-stu-id="34edb-193">String</span></span>|<span data-ttu-id="34edb-194">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="34edb-194">The name of the main Lob application file.</span></span> <span data-ttu-id="34edb-195">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="34edb-195">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="34edb-196">size</span><span class="sxs-lookup"><span data-stu-id="34edb-196">size</span></span>|<span data-ttu-id="34edb-197">Int64</span><span class="sxs-lookup"><span data-stu-id="34edb-197">Int64</span></span>|<span data-ttu-id="34edb-198">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="34edb-198">The total size, including all uploaded files.</span></span> <span data-ttu-id="34edb-199">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="34edb-199">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="34edb-200">commandLine</span><span class="sxs-lookup"><span data-stu-id="34edb-200">commandLine</span></span>|<span data-ttu-id="34edb-201">String</span><span class="sxs-lookup"><span data-stu-id="34edb-201">String</span></span>|<span data-ttu-id="34edb-202">A linha de comando.</span><span class="sxs-lookup"><span data-stu-id="34edb-202">The command line.</span></span>|
|<span data-ttu-id="34edb-203">productCode</span><span class="sxs-lookup"><span data-stu-id="34edb-203">productCode</span></span>|<span data-ttu-id="34edb-204">String</span><span class="sxs-lookup"><span data-stu-id="34edb-204">String</span></span>|<span data-ttu-id="34edb-205">O código do produto.</span><span class="sxs-lookup"><span data-stu-id="34edb-205">The product code.</span></span>|
|<span data-ttu-id="34edb-206">productVersion</span><span class="sxs-lookup"><span data-stu-id="34edb-206">productVersion</span></span>|<span data-ttu-id="34edb-207">String</span><span class="sxs-lookup"><span data-stu-id="34edb-207">String</span></span>|<span data-ttu-id="34edb-208">A versão de produto do aplicativo de linha de negócios (LoB) Windows Mobile MSI.</span><span class="sxs-lookup"><span data-stu-id="34edb-208">The product version of Windows Mobile MSI Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="34edb-209">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="34edb-209">ignoreVersionDetection</span></span>|<span data-ttu-id="34edb-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="34edb-210">Boolean</span></span>|<span data-ttu-id="34edb-211">Um booliano para controlar se a versão do aplicativo será usada para detectar o aplicativo depois que ele for instalado em um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="34edb-211">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="34edb-212">Defina como true para o aplicativos de linha de negócios (LoB) Windows Mobile MSI que usam um recurso de atualização automática.</span><span class="sxs-lookup"><span data-stu-id="34edb-212">Set this to true for Windows Mobile MSI Line of Business (LoB) apps that use a self update feature.</span></span>|



## <a name="response"></a><span data-ttu-id="34edb-213">Resposta</span><span class="sxs-lookup"><span data-stu-id="34edb-213">Response</span></span>
<span data-ttu-id="34edb-214">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="34edb-214">If successful, this method returns a `200 OK` response code and an updated [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34edb-215">Exemplo</span><span class="sxs-lookup"><span data-stu-id="34edb-215">Example</span></span>
### <a name="request"></a><span data-ttu-id="34edb-216">Solicitação</span><span class="sxs-lookup"><span data-stu-id="34edb-216">Request</span></span>
<span data-ttu-id="34edb-217">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="34edb-217">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="34edb-218">Resposta</span><span class="sxs-lookup"><span data-stu-id="34edb-218">Response</span></span>
<span data-ttu-id="34edb-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="34edb-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



