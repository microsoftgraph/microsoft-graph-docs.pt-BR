---
title: Criar macOSLobApp
description: Criar um novo objeto macOSLobApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a82e0d63789a2edef8cf2eb267bafeba29b2117d
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/18/2020
ms.locfileid: "46792111"
---
# <a name="create-macoslobapp"></a><span data-ttu-id="e26d0-103">Criar macOSLobApp</span><span class="sxs-lookup"><span data-stu-id="e26d0-103">Create macOSLobApp</span></span>

<span data-ttu-id="e26d0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e26d0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e26d0-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e26d0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e26d0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e26d0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e26d0-107">Criar um novo objeto [macOSLobApp](../resources/intune-apps-macoslobapp.md) .</span><span class="sxs-lookup"><span data-stu-id="e26d0-107">Create a new [macOSLobApp](../resources/intune-apps-macoslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e26d0-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e26d0-108">Prerequisites</span></span>
<span data-ttu-id="e26d0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e26d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e26d0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e26d0-111">Permission type</span></span>|<span data-ttu-id="e26d0-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e26d0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e26d0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e26d0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e26d0-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e26d0-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e26d0-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e26d0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e26d0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e26d0-116">Not supported.</span></span>|
|<span data-ttu-id="e26d0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e26d0-117">Application</span></span>|<span data-ttu-id="e26d0-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e26d0-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e26d0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e26d0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="e26d0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e26d0-120">Request headers</span></span>
|<span data-ttu-id="e26d0-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e26d0-121">Header</span></span>|<span data-ttu-id="e26d0-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e26d0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e26d0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e26d0-123">Authorization</span></span>|<span data-ttu-id="e26d0-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e26d0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e26d0-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e26d0-125">Accept</span></span>|<span data-ttu-id="e26d0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e26d0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e26d0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e26d0-127">Request body</span></span>
<span data-ttu-id="e26d0-128">No corpo da solicitação, forneça uma representação JSON do objeto macOSLobApp.</span><span class="sxs-lookup"><span data-stu-id="e26d0-128">In the request body, supply a JSON representation for the macOSLobApp object.</span></span>

<span data-ttu-id="e26d0-129">A tabela a seguir mostra as propriedades que são necessárias ao criar macOSLobApp.</span><span class="sxs-lookup"><span data-stu-id="e26d0-129">The following table shows the properties that are required when you create the macOSLobApp.</span></span>

|<span data-ttu-id="e26d0-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e26d0-130">Property</span></span>|<span data-ttu-id="e26d0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e26d0-131">Type</span></span>|<span data-ttu-id="e26d0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e26d0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e26d0-133">id</span><span class="sxs-lookup"><span data-stu-id="e26d0-133">id</span></span>|<span data-ttu-id="e26d0-134">String</span><span class="sxs-lookup"><span data-stu-id="e26d0-134">String</span></span>|<span data-ttu-id="e26d0-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e26d0-135">Key of the entity.</span></span> <span data-ttu-id="e26d0-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e26d0-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e26d0-137">displayName</span><span class="sxs-lookup"><span data-stu-id="e26d0-137">displayName</span></span>|<span data-ttu-id="e26d0-138">String</span><span class="sxs-lookup"><span data-stu-id="e26d0-138">String</span></span>|<span data-ttu-id="e26d0-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="e26d0-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="e26d0-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e26d0-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e26d0-141">description</span><span class="sxs-lookup"><span data-stu-id="e26d0-141">description</span></span>|<span data-ttu-id="e26d0-142">String</span><span class="sxs-lookup"><span data-stu-id="e26d0-142">String</span></span>|<span data-ttu-id="e26d0-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e26d0-143">The description of the app.</span></span> <span data-ttu-id="e26d0-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e26d0-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e26d0-145">publicador</span><span class="sxs-lookup"><span data-stu-id="e26d0-145">publisher</span></span>|<span data-ttu-id="e26d0-146">String</span><span class="sxs-lookup"><span data-stu-id="e26d0-146">String</span></span>|<span data-ttu-id="e26d0-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e26d0-147">The publisher of the app.</span></span> <span data-ttu-id="e26d0-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e26d0-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e26d0-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e26d0-149">largeIcon</span></span>|[<span data-ttu-id="e26d0-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e26d0-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e26d0-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="e26d0-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="e26d0-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e26d0-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e26d0-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e26d0-153">createdDateTime</span></span>|<span data-ttu-id="e26d0-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e26d0-154">DateTimeOffset</span></span>|<span data-ttu-id="e26d0-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e26d0-155">The date and time the app was created.</span></span> <span data-ttu-id="e26d0-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e26d0-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e26d0-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e26d0-157">lastModifiedDateTime</span></span>|<span data-ttu-id="e26d0-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e26d0-158">DateTimeOffset</span></span>|<span data-ttu-id="e26d0-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="e26d0-159">The date and time the app was last modified.</span></span> <span data-ttu-id="e26d0-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e26d0-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e26d0-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e26d0-161">isFeatured</span></span>|<span data-ttu-id="e26d0-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="e26d0-162">Boolean</span></span>|<span data-ttu-id="e26d0-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e26d0-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e26d0-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e26d0-164">privacyInformationUrl</span></span>|<span data-ttu-id="e26d0-165">String</span><span class="sxs-lookup"><span data-stu-id="e26d0-165">String</span></span>|<span data-ttu-id="e26d0-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="e26d0-166">The privacy statement Url.</span></span> <span data-ttu-id="e26d0-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e26d0-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e26d0-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e26d0-168">informationUrl</span></span>|<span data-ttu-id="e26d0-169">String</span><span class="sxs-lookup"><span data-stu-id="e26d0-169">String</span></span>|<span data-ttu-id="e26d0-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="e26d0-170">The more information Url.</span></span> <span data-ttu-id="e26d0-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e26d0-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e26d0-172">owner</span><span class="sxs-lookup"><span data-stu-id="e26d0-172">owner</span></span>|<span data-ttu-id="e26d0-173">String</span><span class="sxs-lookup"><span data-stu-id="e26d0-173">String</span></span>|<span data-ttu-id="e26d0-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="e26d0-174">The owner of the app.</span></span> <span data-ttu-id="e26d0-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e26d0-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e26d0-176">developer</span><span class="sxs-lookup"><span data-stu-id="e26d0-176">developer</span></span>|<span data-ttu-id="e26d0-177">String</span><span class="sxs-lookup"><span data-stu-id="e26d0-177">String</span></span>|<span data-ttu-id="e26d0-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e26d0-178">The developer of the app.</span></span> <span data-ttu-id="e26d0-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e26d0-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e26d0-180">notes</span><span class="sxs-lookup"><span data-stu-id="e26d0-180">notes</span></span>|<span data-ttu-id="e26d0-181">String</span><span class="sxs-lookup"><span data-stu-id="e26d0-181">String</span></span>|<span data-ttu-id="e26d0-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e26d0-182">Notes for the app.</span></span> <span data-ttu-id="e26d0-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e26d0-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e26d0-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="e26d0-184">uploadState</span></span>|<span data-ttu-id="e26d0-185">Int32</span><span class="sxs-lookup"><span data-stu-id="e26d0-185">Int32</span></span>|<span data-ttu-id="e26d0-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="e26d0-186">The upload state.</span></span> <span data-ttu-id="e26d0-187">Os valores possíveis são: 0- `Not Ready` , 1- `Ready` , 2- `Processing` .</span><span class="sxs-lookup"><span data-stu-id="e26d0-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="e26d0-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e26d0-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e26d0-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="e26d0-189">publishingState</span></span>|[<span data-ttu-id="e26d0-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="e26d0-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="e26d0-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e26d0-191">The publishing state for the app.</span></span> <span data-ttu-id="e26d0-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="e26d0-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="e26d0-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e26d0-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="e26d0-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="e26d0-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="e26d0-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="e26d0-195">isAssigned</span></span>|<span data-ttu-id="e26d0-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="e26d0-196">Boolean</span></span>|<span data-ttu-id="e26d0-197">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="e26d0-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="e26d0-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e26d0-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e26d0-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e26d0-199">roleScopeTagIds</span></span>|<span data-ttu-id="e26d0-200">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e26d0-200">String collection</span></span>|<span data-ttu-id="e26d0-201">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="e26d0-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="e26d0-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e26d0-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e26d0-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="e26d0-203">dependentAppCount</span></span>|<span data-ttu-id="e26d0-204">Int32</span><span class="sxs-lookup"><span data-stu-id="e26d0-204">Int32</span></span>|<span data-ttu-id="e26d0-205">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="e26d0-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="e26d0-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e26d0-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e26d0-207">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="e26d0-207">committedContentVersion</span></span>|<span data-ttu-id="e26d0-208">String</span><span class="sxs-lookup"><span data-stu-id="e26d0-208">String</span></span>|<span data-ttu-id="e26d0-209">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="e26d0-209">The internal committed content version.</span></span> <span data-ttu-id="e26d0-210">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="e26d0-210">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e26d0-211">fileName</span><span class="sxs-lookup"><span data-stu-id="e26d0-211">fileName</span></span>|<span data-ttu-id="e26d0-212">String</span><span class="sxs-lookup"><span data-stu-id="e26d0-212">String</span></span>|<span data-ttu-id="e26d0-213">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="e26d0-213">The name of the main Lob application file.</span></span> <span data-ttu-id="e26d0-214">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="e26d0-214">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e26d0-215">size</span><span class="sxs-lookup"><span data-stu-id="e26d0-215">size</span></span>|<span data-ttu-id="e26d0-216">Int64</span><span class="sxs-lookup"><span data-stu-id="e26d0-216">Int64</span></span>|<span data-ttu-id="e26d0-217">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="e26d0-217">The total size, including all uploaded files.</span></span> <span data-ttu-id="e26d0-218">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="e26d0-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e26d0-219">bundleId</span><span class="sxs-lookup"><span data-stu-id="e26d0-219">bundleId</span></span>|<span data-ttu-id="e26d0-220">String</span><span class="sxs-lookup"><span data-stu-id="e26d0-220">String</span></span>|<span data-ttu-id="e26d0-221">A ID do pacote.</span><span class="sxs-lookup"><span data-stu-id="e26d0-221">The bundle id.</span></span>|
|<span data-ttu-id="e26d0-222">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e26d0-222">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="e26d0-223">macOSMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e26d0-223">macOSMinimumOperatingSystem</span></span>](../resources/intune-apps-macosminimumoperatingsystem.md)|<span data-ttu-id="e26d0-224">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="e26d0-224">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="e26d0-225">buildNumber</span><span class="sxs-lookup"><span data-stu-id="e26d0-225">buildNumber</span></span>|<span data-ttu-id="e26d0-226">String</span><span class="sxs-lookup"><span data-stu-id="e26d0-226">String</span></span>|<span data-ttu-id="e26d0-227">O número de compilação do aplicativo de linha de negócios (LoB) MacOS.</span><span class="sxs-lookup"><span data-stu-id="e26d0-227">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="e26d0-228">versionNumber</span><span class="sxs-lookup"><span data-stu-id="e26d0-228">versionNumber</span></span>|<span data-ttu-id="e26d0-229">String</span><span class="sxs-lookup"><span data-stu-id="e26d0-229">String</span></span>|<span data-ttu-id="e26d0-230">O número da versão do aplicativo de linha de negócios (LoB) MacOS.</span><span class="sxs-lookup"><span data-stu-id="e26d0-230">The version number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="e26d0-231">childApps</span><span class="sxs-lookup"><span data-stu-id="e26d0-231">childApps</span></span>|<span data-ttu-id="e26d0-232">coleção [macOSLobChildApp](../resources/intune-apps-macoslobchildapp.md)</span><span class="sxs-lookup"><span data-stu-id="e26d0-232">[macOSLobChildApp](../resources/intune-apps-macoslobchildapp.md) collection</span></span>|<span data-ttu-id="e26d0-233">A lista de aplicativos neste pacote de pacotes</span><span class="sxs-lookup"><span data-stu-id="e26d0-233">The app list in this bundle package</span></span>|
|<span data-ttu-id="e26d0-234">identityVersion</span><span class="sxs-lookup"><span data-stu-id="e26d0-234">identityVersion</span></span>|<span data-ttu-id="e26d0-235">String</span><span class="sxs-lookup"><span data-stu-id="e26d0-235">String</span></span>|<span data-ttu-id="e26d0-236">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="e26d0-236">The identity version.</span></span>|
|<span data-ttu-id="e26d0-237">md5HashChunkSize</span><span class="sxs-lookup"><span data-stu-id="e26d0-237">md5HashChunkSize</span></span>|<span data-ttu-id="e26d0-238">Int32</span><span class="sxs-lookup"><span data-stu-id="e26d0-238">Int32</span></span>|<span data-ttu-id="e26d0-239">O tamanho da parte do hash MD5</span><span class="sxs-lookup"><span data-stu-id="e26d0-239">The chunk size for MD5 hash</span></span>|
|<span data-ttu-id="e26d0-240">md5Hash</span><span class="sxs-lookup"><span data-stu-id="e26d0-240">md5Hash</span></span>|<span data-ttu-id="e26d0-241">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e26d0-241">String collection</span></span>|<span data-ttu-id="e26d0-242">Os códigos de hash MD5</span><span class="sxs-lookup"><span data-stu-id="e26d0-242">The MD5 hash codes</span></span>|
|<span data-ttu-id="e26d0-243">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="e26d0-243">ignoreVersionDetection</span></span>|<span data-ttu-id="e26d0-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="e26d0-244">Boolean</span></span>|<span data-ttu-id="e26d0-245">Um booliano para controlar se a versão do aplicativo será usada para detectar o aplicativo depois que ele for instalado em um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e26d0-245">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="e26d0-246">Defina isso como true para aplicativos de linha de negócios (LoB) de macOS que usam um recurso de autoatualização.</span><span class="sxs-lookup"><span data-stu-id="e26d0-246">Set this to true for macOS Line of Business (LoB) apps that use a self update feature.</span></span>|



## <a name="response"></a><span data-ttu-id="e26d0-247">Resposta</span><span class="sxs-lookup"><span data-stu-id="e26d0-247">Response</span></span>
<span data-ttu-id="e26d0-248">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [macOSLobApp](../resources/intune-apps-macoslobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e26d0-248">If successful, this method returns a `201 Created` response code and a [macOSLobApp](../resources/intune-apps-macoslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e26d0-249">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e26d0-249">Example</span></span>

### <a name="request"></a><span data-ttu-id="e26d0-250">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e26d0-250">Request</span></span>
<span data-ttu-id="e26d0-251">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e26d0-251">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1616

{
  "@odata.type": "#microsoft.graph.macOSLobApp",
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
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "dependentAppCount": 1,
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "bundleId": "Bundle Id value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.macOSMinimumOperatingSystem",
    "v10_7": true,
    "v10_8": true,
    "v10_9": true,
    "v10_10": true,
    "v10_11": true,
    "v10_12": true,
    "v10_13": true,
    "v10_14": true,
    "v10_15": true
  },
  "buildNumber": "Build Number value",
  "versionNumber": "Version Number value",
  "childApps": [
    {
      "@odata.type": "microsoft.graph.macOSLobChildApp",
      "bundleId": "Bundle Id value",
      "buildNumber": "Build Number value",
      "versionNumber": "Version Number value"
    }
  ],
  "identityVersion": "Identity Version value",
  "md5HashChunkSize": 0,
  "md5Hash": [
    "Md5Hash value"
  ],
  "ignoreVersionDetection": true
}
```

### <a name="response"></a><span data-ttu-id="e26d0-252">Resposta</span><span class="sxs-lookup"><span data-stu-id="e26d0-252">Response</span></span>
<span data-ttu-id="e26d0-p123">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e26d0-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1788

{
  "@odata.type": "#microsoft.graph.macOSLobApp",
  "id": "7be9250a-250a-7be9-0a25-e97b0a25e97b",
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
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "dependentAppCount": 1,
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "bundleId": "Bundle Id value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.macOSMinimumOperatingSystem",
    "v10_7": true,
    "v10_8": true,
    "v10_9": true,
    "v10_10": true,
    "v10_11": true,
    "v10_12": true,
    "v10_13": true,
    "v10_14": true,
    "v10_15": true
  },
  "buildNumber": "Build Number value",
  "versionNumber": "Version Number value",
  "childApps": [
    {
      "@odata.type": "microsoft.graph.macOSLobChildApp",
      "bundleId": "Bundle Id value",
      "buildNumber": "Build Number value",
      "versionNumber": "Version Number value"
    }
  ],
  "identityVersion": "Identity Version value",
  "md5HashChunkSize": 0,
  "md5Hash": [
    "Md5Hash value"
  ],
  "ignoreVersionDetection": true
}
```



