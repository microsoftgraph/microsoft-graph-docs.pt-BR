---
title: Criar androidLobApp
description: Cria um novo objeto androidLobApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8f20b79f14f9dfd92a9615a5f1d65e073f20d069
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32577557"
---
# <a name="create-androidlobapp"></a><span data-ttu-id="c76f4-103">Criar androidLobApp</span><span class="sxs-lookup"><span data-stu-id="c76f4-103">Create androidLobApp</span></span>

> <span data-ttu-id="c76f4-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c76f4-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c76f4-105">Cria um novo objeto [androidLobApp](../resources/intune-apps-androidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="c76f4-105">Create a new [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c76f4-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c76f4-106">Prerequisites</span></span>
<span data-ttu-id="c76f4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c76f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c76f4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c76f4-109">Permission type</span></span>|<span data-ttu-id="c76f4-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c76f4-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c76f4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c76f4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c76f4-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c76f4-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c76f4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c76f4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c76f4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c76f4-114">Not supported.</span></span>|
|<span data-ttu-id="c76f4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c76f4-115">Application</span></span>|<span data-ttu-id="c76f4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c76f4-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c76f4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c76f4-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="c76f4-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c76f4-118">Request headers</span></span>
|<span data-ttu-id="c76f4-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c76f4-119">Header</span></span>|<span data-ttu-id="c76f4-120">Valor</span><span class="sxs-lookup"><span data-stu-id="c76f4-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c76f4-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c76f4-121">Authorization</span></span>|<span data-ttu-id="c76f4-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c76f4-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c76f4-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c76f4-123">Accept</span></span>|<span data-ttu-id="c76f4-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c76f4-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c76f4-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c76f4-125">Request body</span></span>
<span data-ttu-id="c76f4-126">No corpo da solicitação, forneça uma representação JSON do objeto androidLobApp.</span><span class="sxs-lookup"><span data-stu-id="c76f4-126">In the request body, supply a JSON representation for the androidLobApp object.</span></span>

<span data-ttu-id="c76f4-127">A tabela a seguir mostra as propriedades obrigatórias ao criar androidLobApp.</span><span class="sxs-lookup"><span data-stu-id="c76f4-127">The following table shows the properties that are required when you create the androidLobApp.</span></span>

|<span data-ttu-id="c76f4-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c76f4-128">Property</span></span>|<span data-ttu-id="c76f4-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="c76f4-129">Type</span></span>|<span data-ttu-id="c76f4-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="c76f4-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c76f4-131">id</span><span class="sxs-lookup"><span data-stu-id="c76f4-131">id</span></span>|<span data-ttu-id="c76f4-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c76f4-132">String</span></span>|<span data-ttu-id="c76f4-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c76f4-133">Key of the entity.</span></span> <span data-ttu-id="c76f4-134">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c76f4-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c76f4-135">displayName</span><span class="sxs-lookup"><span data-stu-id="c76f4-135">displayName</span></span>|<span data-ttu-id="c76f4-136">String</span><span class="sxs-lookup"><span data-stu-id="c76f4-136">String</span></span>|<span data-ttu-id="c76f4-137">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="c76f4-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="c76f4-138">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c76f4-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c76f4-139">description</span><span class="sxs-lookup"><span data-stu-id="c76f4-139">description</span></span>|<span data-ttu-id="c76f4-140">String</span><span class="sxs-lookup"><span data-stu-id="c76f4-140">String</span></span>|<span data-ttu-id="c76f4-141">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c76f4-141">The description of the app.</span></span> <span data-ttu-id="c76f4-142">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c76f4-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c76f4-143">publicador</span><span class="sxs-lookup"><span data-stu-id="c76f4-143">publisher</span></span>|<span data-ttu-id="c76f4-144">String</span><span class="sxs-lookup"><span data-stu-id="c76f4-144">String</span></span>|<span data-ttu-id="c76f4-145">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c76f4-145">The publisher of the app.</span></span> <span data-ttu-id="c76f4-146">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c76f4-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c76f4-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="c76f4-147">largeIcon</span></span>|[<span data-ttu-id="c76f4-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="c76f4-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="c76f4-149">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="c76f4-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="c76f4-150">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c76f4-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c76f4-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c76f4-151">createdDateTime</span></span>|<span data-ttu-id="c76f4-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c76f4-152">DateTimeOffset</span></span>|<span data-ttu-id="c76f4-153">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c76f4-153">The date and time the app was created.</span></span> <span data-ttu-id="c76f4-154">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c76f4-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c76f4-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c76f4-155">lastModifiedDateTime</span></span>|<span data-ttu-id="c76f4-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c76f4-156">DateTimeOffset</span></span>|<span data-ttu-id="c76f4-157">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="c76f4-157">The date and time the app was last modified.</span></span> <span data-ttu-id="c76f4-158">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c76f4-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c76f4-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="c76f4-159">isFeatured</span></span>|<span data-ttu-id="c76f4-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="c76f4-160">Boolean</span></span>|<span data-ttu-id="c76f4-161">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c76f4-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c76f4-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="c76f4-162">privacyInformationUrl</span></span>|<span data-ttu-id="c76f4-163">String</span><span class="sxs-lookup"><span data-stu-id="c76f4-163">String</span></span>|<span data-ttu-id="c76f4-164">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="c76f4-164">The privacy statement Url.</span></span> <span data-ttu-id="c76f4-165">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c76f4-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c76f4-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="c76f4-166">informationUrl</span></span>|<span data-ttu-id="c76f4-167">String</span><span class="sxs-lookup"><span data-stu-id="c76f4-167">String</span></span>|<span data-ttu-id="c76f4-168">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="c76f4-168">The more information Url.</span></span> <span data-ttu-id="c76f4-169">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c76f4-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c76f4-170">owner</span><span class="sxs-lookup"><span data-stu-id="c76f4-170">owner</span></span>|<span data-ttu-id="c76f4-171">String</span><span class="sxs-lookup"><span data-stu-id="c76f4-171">String</span></span>|<span data-ttu-id="c76f4-172">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="c76f4-172">The owner of the app.</span></span> <span data-ttu-id="c76f4-173">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c76f4-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c76f4-174">developer</span><span class="sxs-lookup"><span data-stu-id="c76f4-174">developer</span></span>|<span data-ttu-id="c76f4-175">String</span><span class="sxs-lookup"><span data-stu-id="c76f4-175">String</span></span>|<span data-ttu-id="c76f4-176">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c76f4-176">The developer of the app.</span></span> <span data-ttu-id="c76f4-177">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c76f4-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c76f4-178">notes</span><span class="sxs-lookup"><span data-stu-id="c76f4-178">notes</span></span>|<span data-ttu-id="c76f4-179">String</span><span class="sxs-lookup"><span data-stu-id="c76f4-179">String</span></span>|<span data-ttu-id="c76f4-180">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c76f4-180">Notes for the app.</span></span> <span data-ttu-id="c76f4-181">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c76f4-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c76f4-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="c76f4-182">publishingState</span></span>|[<span data-ttu-id="c76f4-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="c76f4-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="c76f4-184">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c76f4-184">The publishing state for the app.</span></span> <span data-ttu-id="c76f4-185">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="c76f4-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="c76f4-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c76f4-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="c76f4-187">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="c76f4-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="c76f4-188">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="c76f4-188">committedContentVersion</span></span>|<span data-ttu-id="c76f4-189">String</span><span class="sxs-lookup"><span data-stu-id="c76f4-189">String</span></span>|<span data-ttu-id="c76f4-190">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="c76f4-190">The internal committed content version.</span></span> <span data-ttu-id="c76f4-191">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="c76f4-191">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="c76f4-192">fileName</span><span class="sxs-lookup"><span data-stu-id="c76f4-192">fileName</span></span>|<span data-ttu-id="c76f4-193">String</span><span class="sxs-lookup"><span data-stu-id="c76f4-193">String</span></span>|<span data-ttu-id="c76f4-194">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="c76f4-194">The name of the main Lob application file.</span></span> <span data-ttu-id="c76f4-195">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="c76f4-195">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="c76f4-196">size</span><span class="sxs-lookup"><span data-stu-id="c76f4-196">size</span></span>|<span data-ttu-id="c76f4-197">Int64</span><span class="sxs-lookup"><span data-stu-id="c76f4-197">Int64</span></span>|<span data-ttu-id="c76f4-198">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="c76f4-198">The total size, including all uploaded files.</span></span> <span data-ttu-id="c76f4-199">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="c76f4-199">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="c76f4-200">packageId</span><span class="sxs-lookup"><span data-stu-id="c76f4-200">packageId</span></span>|<span data-ttu-id="c76f4-201">String</span><span class="sxs-lookup"><span data-stu-id="c76f4-201">String</span></span>|<span data-ttu-id="c76f4-202">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="c76f4-202">The package identifier.</span></span>|
|<span data-ttu-id="c76f4-203">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="c76f4-203">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="c76f4-204">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="c76f4-204">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="c76f4-205">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="c76f4-205">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="c76f4-206">versionName</span><span class="sxs-lookup"><span data-stu-id="c76f4-206">versionName</span></span>|<span data-ttu-id="c76f4-207">String</span><span class="sxs-lookup"><span data-stu-id="c76f4-207">String</span></span>|<span data-ttu-id="c76f4-208">O nome da versão do aplicativo de Linha de Negócios (LoB) Android.</span><span class="sxs-lookup"><span data-stu-id="c76f4-208">The version name of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="c76f4-209">versionCode</span><span class="sxs-lookup"><span data-stu-id="c76f4-209">versionCode</span></span>|<span data-ttu-id="c76f4-210">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c76f4-210">String</span></span>|<span data-ttu-id="c76f4-211">O código da versão do aplicativo de Linha de Negócios (LoB) Android.</span><span class="sxs-lookup"><span data-stu-id="c76f4-211">The version code of Android Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="c76f4-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="c76f4-212">Response</span></span>
<span data-ttu-id="c76f4-213">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [androidLobApp](../resources/intune-apps-androidlobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c76f4-213">If successful, this method returns a `201 Created` response code and a [androidLobApp](../resources/intune-apps-androidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c76f4-214">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c76f4-214">Example</span></span>

### <a name="request"></a><span data-ttu-id="c76f4-215">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c76f4-215">Request</span></span>
<span data-ttu-id="c76f4-216">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c76f4-216">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c76f4-217">Resposta</span><span class="sxs-lookup"><span data-stu-id="c76f4-217">Response</span></span>
<span data-ttu-id="c76f4-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c76f4-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



