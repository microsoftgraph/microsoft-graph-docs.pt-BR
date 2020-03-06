---
title: Atualizar androidLobApp
description: Atualiza as propriedades de um objeto androidLobApp.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ca5c8b1242e5805b00150ebfc79ba0d88499d241
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42516662"
---
# <a name="update-androidlobapp"></a><span data-ttu-id="293b5-103">Atualizar androidLobApp</span><span class="sxs-lookup"><span data-stu-id="293b5-103">Update androidLobApp</span></span>

<span data-ttu-id="293b5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="293b5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="293b5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="293b5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="293b5-106">Atualiza as propriedades de um objeto [androidLobApp](../resources/intune-apps-androidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="293b5-106">Update the properties of a [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="293b5-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="293b5-107">Prerequisites</span></span>
<span data-ttu-id="293b5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="293b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="293b5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="293b5-110">Permission type</span></span>|<span data-ttu-id="293b5-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="293b5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="293b5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="293b5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="293b5-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="293b5-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="293b5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="293b5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="293b5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="293b5-115">Not supported.</span></span>|
|<span data-ttu-id="293b5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="293b5-116">Application</span></span>|<span data-ttu-id="293b5-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="293b5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="293b5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="293b5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="293b5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="293b5-119">Request headers</span></span>
|<span data-ttu-id="293b5-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="293b5-120">Header</span></span>|<span data-ttu-id="293b5-121">Valor</span><span class="sxs-lookup"><span data-stu-id="293b5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="293b5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="293b5-122">Authorization</span></span>|<span data-ttu-id="293b5-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="293b5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="293b5-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="293b5-124">Accept</span></span>|<span data-ttu-id="293b5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="293b5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="293b5-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="293b5-126">Request body</span></span>
<span data-ttu-id="293b5-127">No corpo da solicitação, forneça uma representação JSON do objeto [androidLobApp](../resources/intune-apps-androidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="293b5-127">In the request body, supply a JSON representation for the [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>

<span data-ttu-id="293b5-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [androidLobApp](../resources/intune-apps-androidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="293b5-128">The following table shows the properties that are required when you create the [androidLobApp](../resources/intune-apps-androidlobapp.md).</span></span>

|<span data-ttu-id="293b5-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="293b5-129">Property</span></span>|<span data-ttu-id="293b5-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="293b5-130">Type</span></span>|<span data-ttu-id="293b5-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="293b5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="293b5-132">id</span><span class="sxs-lookup"><span data-stu-id="293b5-132">id</span></span>|<span data-ttu-id="293b5-133">String</span><span class="sxs-lookup"><span data-stu-id="293b5-133">String</span></span>|<span data-ttu-id="293b5-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="293b5-134">Key of the entity.</span></span> <span data-ttu-id="293b5-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="293b5-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="293b5-136">displayName</span><span class="sxs-lookup"><span data-stu-id="293b5-136">displayName</span></span>|<span data-ttu-id="293b5-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="293b5-137">String</span></span>|<span data-ttu-id="293b5-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="293b5-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="293b5-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="293b5-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="293b5-140">description</span><span class="sxs-lookup"><span data-stu-id="293b5-140">description</span></span>|<span data-ttu-id="293b5-141">String</span><span class="sxs-lookup"><span data-stu-id="293b5-141">String</span></span>|<span data-ttu-id="293b5-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="293b5-142">The description of the app.</span></span> <span data-ttu-id="293b5-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="293b5-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="293b5-144">publicador</span><span class="sxs-lookup"><span data-stu-id="293b5-144">publisher</span></span>|<span data-ttu-id="293b5-145">String</span><span class="sxs-lookup"><span data-stu-id="293b5-145">String</span></span>|<span data-ttu-id="293b5-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="293b5-146">The publisher of the app.</span></span> <span data-ttu-id="293b5-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="293b5-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="293b5-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="293b5-148">largeIcon</span></span>|[<span data-ttu-id="293b5-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="293b5-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="293b5-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="293b5-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="293b5-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="293b5-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="293b5-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="293b5-152">createdDateTime</span></span>|<span data-ttu-id="293b5-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="293b5-153">DateTimeOffset</span></span>|<span data-ttu-id="293b5-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="293b5-154">The date and time the app was created.</span></span> <span data-ttu-id="293b5-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="293b5-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="293b5-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="293b5-156">lastModifiedDateTime</span></span>|<span data-ttu-id="293b5-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="293b5-157">DateTimeOffset</span></span>|<span data-ttu-id="293b5-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="293b5-158">The date and time the app was last modified.</span></span> <span data-ttu-id="293b5-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="293b5-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="293b5-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="293b5-160">isFeatured</span></span>|<span data-ttu-id="293b5-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="293b5-161">Boolean</span></span>|<span data-ttu-id="293b5-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="293b5-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="293b5-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="293b5-163">privacyInformationUrl</span></span>|<span data-ttu-id="293b5-164">String</span><span class="sxs-lookup"><span data-stu-id="293b5-164">String</span></span>|<span data-ttu-id="293b5-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="293b5-165">The privacy statement Url.</span></span> <span data-ttu-id="293b5-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="293b5-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="293b5-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="293b5-167">informationUrl</span></span>|<span data-ttu-id="293b5-168">String</span><span class="sxs-lookup"><span data-stu-id="293b5-168">String</span></span>|<span data-ttu-id="293b5-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="293b5-169">The more information Url.</span></span> <span data-ttu-id="293b5-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="293b5-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="293b5-171">owner</span><span class="sxs-lookup"><span data-stu-id="293b5-171">owner</span></span>|<span data-ttu-id="293b5-172">String</span><span class="sxs-lookup"><span data-stu-id="293b5-172">String</span></span>|<span data-ttu-id="293b5-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="293b5-173">The owner of the app.</span></span> <span data-ttu-id="293b5-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="293b5-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="293b5-175">developer</span><span class="sxs-lookup"><span data-stu-id="293b5-175">developer</span></span>|<span data-ttu-id="293b5-176">String</span><span class="sxs-lookup"><span data-stu-id="293b5-176">String</span></span>|<span data-ttu-id="293b5-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="293b5-177">The developer of the app.</span></span> <span data-ttu-id="293b5-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="293b5-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="293b5-179">notes</span><span class="sxs-lookup"><span data-stu-id="293b5-179">notes</span></span>|<span data-ttu-id="293b5-180">String</span><span class="sxs-lookup"><span data-stu-id="293b5-180">String</span></span>|<span data-ttu-id="293b5-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="293b5-181">Notes for the app.</span></span> <span data-ttu-id="293b5-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="293b5-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="293b5-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="293b5-183">publishingState</span></span>|[<span data-ttu-id="293b5-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="293b5-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="293b5-185">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="293b5-185">The publishing state for the app.</span></span> <span data-ttu-id="293b5-186">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="293b5-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="293b5-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="293b5-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="293b5-188">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="293b5-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="293b5-189">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="293b5-189">committedContentVersion</span></span>|<span data-ttu-id="293b5-190">String</span><span class="sxs-lookup"><span data-stu-id="293b5-190">String</span></span>|<span data-ttu-id="293b5-191">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="293b5-191">The internal committed content version.</span></span> <span data-ttu-id="293b5-192">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="293b5-192">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="293b5-193">fileName</span><span class="sxs-lookup"><span data-stu-id="293b5-193">fileName</span></span>|<span data-ttu-id="293b5-194">String</span><span class="sxs-lookup"><span data-stu-id="293b5-194">String</span></span>|<span data-ttu-id="293b5-195">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="293b5-195">The name of the main Lob application file.</span></span> <span data-ttu-id="293b5-196">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="293b5-196">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="293b5-197">size</span><span class="sxs-lookup"><span data-stu-id="293b5-197">size</span></span>|<span data-ttu-id="293b5-198">Int64</span><span class="sxs-lookup"><span data-stu-id="293b5-198">Int64</span></span>|<span data-ttu-id="293b5-199">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="293b5-199">The total size, including all uploaded files.</span></span> <span data-ttu-id="293b5-200">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="293b5-200">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="293b5-201">packageId</span><span class="sxs-lookup"><span data-stu-id="293b5-201">packageId</span></span>|<span data-ttu-id="293b5-202">String</span><span class="sxs-lookup"><span data-stu-id="293b5-202">String</span></span>|<span data-ttu-id="293b5-203">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="293b5-203">The package identifier.</span></span>|
|<span data-ttu-id="293b5-204">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="293b5-204">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="293b5-205">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="293b5-205">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="293b5-206">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="293b5-206">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="293b5-207">versionName</span><span class="sxs-lookup"><span data-stu-id="293b5-207">versionName</span></span>|<span data-ttu-id="293b5-208">String</span><span class="sxs-lookup"><span data-stu-id="293b5-208">String</span></span>|<span data-ttu-id="293b5-209">O nome da versão do aplicativo de Linha de Negócios (LoB) Android.</span><span class="sxs-lookup"><span data-stu-id="293b5-209">The version name of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="293b5-210">versionCode</span><span class="sxs-lookup"><span data-stu-id="293b5-210">versionCode</span></span>|<span data-ttu-id="293b5-211">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="293b5-211">String</span></span>|<span data-ttu-id="293b5-212">O código da versão do aplicativo de Linha de Negócios (LoB) Android.</span><span class="sxs-lookup"><span data-stu-id="293b5-212">The version code of Android Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="293b5-213">Resposta</span><span class="sxs-lookup"><span data-stu-id="293b5-213">Response</span></span>
<span data-ttu-id="293b5-214">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [androidLobApp](../resources/intune-apps-androidlobapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="293b5-214">If successful, this method returns a `200 OK` response code and an updated [androidLobApp](../resources/intune-apps-androidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="293b5-215">Exemplo</span><span class="sxs-lookup"><span data-stu-id="293b5-215">Example</span></span>

### <a name="request"></a><span data-ttu-id="293b5-216">Solicitação</span><span class="sxs-lookup"><span data-stu-id="293b5-216">Request</span></span>
<span data-ttu-id="293b5-217">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="293b5-217">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="293b5-218">Resposta</span><span class="sxs-lookup"><span data-stu-id="293b5-218">Response</span></span>
<span data-ttu-id="293b5-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="293b5-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




