---
title: Criar androidLobApp
description: Cria um novo objeto androidLobApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6c68bc7e7a5bb07228e6afd40d7bfe5c50fdd6c3
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30257936"
---
# <a name="create-androidlobapp"></a><span data-ttu-id="fc7d8-103">Criar androidLobApp</span><span class="sxs-lookup"><span data-stu-id="fc7d8-103">Create androidLobApp</span></span>

> <span data-ttu-id="fc7d8-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fc7d8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc7d8-105">Cria um novo objeto [androidLobApp](../resources/intune-apps-androidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="fc7d8-105">Create a new [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fc7d8-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fc7d8-106">Prerequisites</span></span>
<span data-ttu-id="fc7d8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="fc7d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fc7d8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fc7d8-109">Permission type</span></span>|<span data-ttu-id="fc7d8-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fc7d8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fc7d8-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fc7d8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fc7d8-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc7d8-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fc7d8-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fc7d8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fc7d8-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fc7d8-114">Not supported.</span></span>|
|<span data-ttu-id="fc7d8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fc7d8-115">Application</span></span>|<span data-ttu-id="fc7d8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fc7d8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fc7d8-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fc7d8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="fc7d8-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fc7d8-118">Request headers</span></span>
|<span data-ttu-id="fc7d8-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fc7d8-119">Header</span></span>|<span data-ttu-id="fc7d8-120">Valor</span><span class="sxs-lookup"><span data-stu-id="fc7d8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fc7d8-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="fc7d8-121">Authorization</span></span>|<span data-ttu-id="fc7d8-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fc7d8-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fc7d8-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fc7d8-123">Accept</span></span>|<span data-ttu-id="fc7d8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="fc7d8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc7d8-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fc7d8-125">Request body</span></span>
<span data-ttu-id="fc7d8-126">No corpo da solicitação, forneça uma representação JSON do objeto androidLobApp.</span><span class="sxs-lookup"><span data-stu-id="fc7d8-126">In the request body, supply a JSON representation for the androidLobApp object.</span></span>

<span data-ttu-id="fc7d8-127">A tabela a seguir mostra as propriedades obrigatórias ao criar androidLobApp.</span><span class="sxs-lookup"><span data-stu-id="fc7d8-127">The following table shows the properties that are required when you create the androidLobApp.</span></span>

|<span data-ttu-id="fc7d8-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fc7d8-128">Property</span></span>|<span data-ttu-id="fc7d8-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="fc7d8-129">Type</span></span>|<span data-ttu-id="fc7d8-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc7d8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc7d8-131">id</span><span class="sxs-lookup"><span data-stu-id="fc7d8-131">id</span></span>|<span data-ttu-id="fc7d8-132">String</span><span class="sxs-lookup"><span data-stu-id="fc7d8-132">String</span></span>|<span data-ttu-id="fc7d8-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="fc7d8-133">Key of the entity.</span></span> <span data-ttu-id="fc7d8-134">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc7d8-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fc7d8-135">displayName</span><span class="sxs-lookup"><span data-stu-id="fc7d8-135">displayName</span></span>|<span data-ttu-id="fc7d8-136">String</span><span class="sxs-lookup"><span data-stu-id="fc7d8-136">String</span></span>|<span data-ttu-id="fc7d8-137">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="fc7d8-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="fc7d8-138">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc7d8-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fc7d8-139">description</span><span class="sxs-lookup"><span data-stu-id="fc7d8-139">description</span></span>|<span data-ttu-id="fc7d8-140">String</span><span class="sxs-lookup"><span data-stu-id="fc7d8-140">String</span></span>|<span data-ttu-id="fc7d8-141">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fc7d8-141">The description of the app.</span></span> <span data-ttu-id="fc7d8-142">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc7d8-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fc7d8-143">publisher</span><span class="sxs-lookup"><span data-stu-id="fc7d8-143">publisher</span></span>|<span data-ttu-id="fc7d8-144">String</span><span class="sxs-lookup"><span data-stu-id="fc7d8-144">String</span></span>|<span data-ttu-id="fc7d8-145">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fc7d8-145">The publisher of the app.</span></span> <span data-ttu-id="fc7d8-146">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc7d8-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fc7d8-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="fc7d8-147">largeIcon</span></span>|[<span data-ttu-id="fc7d8-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="fc7d8-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="fc7d8-149">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="fc7d8-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="fc7d8-150">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc7d8-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fc7d8-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fc7d8-151">createdDateTime</span></span>|<span data-ttu-id="fc7d8-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc7d8-152">DateTimeOffset</span></span>|<span data-ttu-id="fc7d8-153">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fc7d8-153">The date and time the app was created.</span></span> <span data-ttu-id="fc7d8-154">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc7d8-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fc7d8-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fc7d8-155">lastModifiedDateTime</span></span>|<span data-ttu-id="fc7d8-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc7d8-156">DateTimeOffset</span></span>|<span data-ttu-id="fc7d8-157">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="fc7d8-157">The date and time the app was last modified.</span></span> <span data-ttu-id="fc7d8-158">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc7d8-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fc7d8-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="fc7d8-159">isFeatured</span></span>|<span data-ttu-id="fc7d8-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc7d8-160">Boolean</span></span>|<span data-ttu-id="fc7d8-161">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc7d8-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fc7d8-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="fc7d8-162">privacyInformationUrl</span></span>|<span data-ttu-id="fc7d8-163">String</span><span class="sxs-lookup"><span data-stu-id="fc7d8-163">String</span></span>|<span data-ttu-id="fc7d8-164">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="fc7d8-164">The privacy statement Url.</span></span> <span data-ttu-id="fc7d8-165">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc7d8-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fc7d8-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="fc7d8-166">informationUrl</span></span>|<span data-ttu-id="fc7d8-167">String</span><span class="sxs-lookup"><span data-stu-id="fc7d8-167">String</span></span>|<span data-ttu-id="fc7d8-168">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="fc7d8-168">The more information Url.</span></span> <span data-ttu-id="fc7d8-169">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc7d8-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fc7d8-170">owner</span><span class="sxs-lookup"><span data-stu-id="fc7d8-170">owner</span></span>|<span data-ttu-id="fc7d8-171">String</span><span class="sxs-lookup"><span data-stu-id="fc7d8-171">String</span></span>|<span data-ttu-id="fc7d8-172">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="fc7d8-172">The owner of the app.</span></span> <span data-ttu-id="fc7d8-173">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc7d8-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fc7d8-174">developer</span><span class="sxs-lookup"><span data-stu-id="fc7d8-174">developer</span></span>|<span data-ttu-id="fc7d8-175">String</span><span class="sxs-lookup"><span data-stu-id="fc7d8-175">String</span></span>|<span data-ttu-id="fc7d8-176">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fc7d8-176">The developer of the app.</span></span> <span data-ttu-id="fc7d8-177">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc7d8-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fc7d8-178">Observações</span><span class="sxs-lookup"><span data-stu-id="fc7d8-178">notes</span></span>|<span data-ttu-id="fc7d8-179">String</span><span class="sxs-lookup"><span data-stu-id="fc7d8-179">String</span></span>|<span data-ttu-id="fc7d8-180">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fc7d8-180">Notes for the app.</span></span> <span data-ttu-id="fc7d8-181">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc7d8-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fc7d8-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="fc7d8-182">publishingState</span></span>|[<span data-ttu-id="fc7d8-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="fc7d8-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="fc7d8-184">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fc7d8-184">The publishing state for the app.</span></span> <span data-ttu-id="fc7d8-185">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="fc7d8-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="fc7d8-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fc7d8-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="fc7d8-187">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="fc7d8-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="fc7d8-188">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="fc7d8-188">committedContentVersion</span></span>|<span data-ttu-id="fc7d8-189">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fc7d8-189">String</span></span>|<span data-ttu-id="fc7d8-190">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="fc7d8-190">The internal committed content version.</span></span> <span data-ttu-id="fc7d8-191">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc7d8-191">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="fc7d8-192">fileName</span><span class="sxs-lookup"><span data-stu-id="fc7d8-192">fileName</span></span>|<span data-ttu-id="fc7d8-193">String</span><span class="sxs-lookup"><span data-stu-id="fc7d8-193">String</span></span>|<span data-ttu-id="fc7d8-194">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="fc7d8-194">The name of the main Lob application file.</span></span> <span data-ttu-id="fc7d8-195">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc7d8-195">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="fc7d8-196">size</span><span class="sxs-lookup"><span data-stu-id="fc7d8-196">size</span></span>|<span data-ttu-id="fc7d8-197">Int64</span><span class="sxs-lookup"><span data-stu-id="fc7d8-197">Int64</span></span>|<span data-ttu-id="fc7d8-198">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="fc7d8-198">The total size, including all uploaded files.</span></span> <span data-ttu-id="fc7d8-199">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc7d8-199">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="fc7d8-200">packageId</span><span class="sxs-lookup"><span data-stu-id="fc7d8-200">packageId</span></span>|<span data-ttu-id="fc7d8-201">String</span><span class="sxs-lookup"><span data-stu-id="fc7d8-201">String</span></span>|<span data-ttu-id="fc7d8-202">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="fc7d8-202">The package identifier.</span></span>|
|<span data-ttu-id="fc7d8-203">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="fc7d8-203">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="fc7d8-204">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="fc7d8-204">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="fc7d8-205">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="fc7d8-205">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="fc7d8-206">versionName</span><span class="sxs-lookup"><span data-stu-id="fc7d8-206">versionName</span></span>|<span data-ttu-id="fc7d8-207">String</span><span class="sxs-lookup"><span data-stu-id="fc7d8-207">String</span></span>|<span data-ttu-id="fc7d8-208">O nome da versão do aplicativo de Linha de Negócios (LoB) Android.</span><span class="sxs-lookup"><span data-stu-id="fc7d8-208">The version name of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="fc7d8-209">versionCode</span><span class="sxs-lookup"><span data-stu-id="fc7d8-209">versionCode</span></span>|<span data-ttu-id="fc7d8-210">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fc7d8-210">String</span></span>|<span data-ttu-id="fc7d8-211">O código da versão do aplicativo de Linha de Negócios (LoB) Android.</span><span class="sxs-lookup"><span data-stu-id="fc7d8-211">The version code of Android Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="fc7d8-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc7d8-212">Response</span></span>
<span data-ttu-id="fc7d8-213">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [androidLobApp](../resources/intune-apps-androidlobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fc7d8-213">If successful, this method returns a `201 Created` response code and a [androidLobApp](../resources/intune-apps-androidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc7d8-214">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fc7d8-214">Example</span></span>

### <a name="request"></a><span data-ttu-id="fc7d8-215">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fc7d8-215">Request</span></span>
<span data-ttu-id="fc7d8-216">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fc7d8-216">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fc7d8-217">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc7d8-217">Response</span></span>
<span data-ttu-id="fc7d8-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fc7d8-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



