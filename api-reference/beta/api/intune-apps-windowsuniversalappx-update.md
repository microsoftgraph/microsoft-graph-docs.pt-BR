---
title: Atualizar windowsUniversalAppX
description: Atualiza as propriedades de um objeto windowsUniversalAppX.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 04300c1d337cd329dcfc5db2ea49418f7f04b866
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37171635"
---
# <a name="update-windowsuniversalappx"></a><span data-ttu-id="e86e8-103">Atualizar windowsUniversalAppX</span><span class="sxs-lookup"><span data-stu-id="e86e8-103">Update windowsUniversalAppX</span></span>

> <span data-ttu-id="e86e8-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e86e8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e86e8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e86e8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e86e8-106">Atualiza as propriedades de um objeto [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="e86e8-106">Update the properties of a [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e86e8-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e86e8-107">Prerequisites</span></span>
<span data-ttu-id="e86e8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e86e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e86e8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e86e8-110">Permission type</span></span>|<span data-ttu-id="e86e8-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e86e8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e86e8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e86e8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e86e8-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e86e8-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e86e8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e86e8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e86e8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e86e8-115">Not supported.</span></span>|
|<span data-ttu-id="e86e8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e86e8-116">Application</span></span>|<span data-ttu-id="e86e8-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e86e8-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e86e8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e86e8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="e86e8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e86e8-119">Request headers</span></span>
|<span data-ttu-id="e86e8-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e86e8-120">Header</span></span>|<span data-ttu-id="e86e8-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e86e8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e86e8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e86e8-122">Authorization</span></span>|<span data-ttu-id="e86e8-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e86e8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e86e8-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e86e8-124">Accept</span></span>|<span data-ttu-id="e86e8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e86e8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e86e8-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e86e8-126">Request body</span></span>
<span data-ttu-id="e86e8-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="e86e8-127">In the request body, supply a JSON representation for the [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

<span data-ttu-id="e86e8-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="e86e8-128">The following table shows the properties that are required when you create the [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span></span>

|<span data-ttu-id="e86e8-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e86e8-129">Property</span></span>|<span data-ttu-id="e86e8-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="e86e8-130">Type</span></span>|<span data-ttu-id="e86e8-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e86e8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e86e8-132">id</span><span class="sxs-lookup"><span data-stu-id="e86e8-132">id</span></span>|<span data-ttu-id="e86e8-133">String</span><span class="sxs-lookup"><span data-stu-id="e86e8-133">String</span></span>|<span data-ttu-id="e86e8-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e86e8-134">Key of the entity.</span></span> <span data-ttu-id="e86e8-135">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e86e8-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e86e8-136">displayName</span><span class="sxs-lookup"><span data-stu-id="e86e8-136">displayName</span></span>|<span data-ttu-id="e86e8-137">String</span><span class="sxs-lookup"><span data-stu-id="e86e8-137">String</span></span>|<span data-ttu-id="e86e8-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="e86e8-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="e86e8-139">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e86e8-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e86e8-140">descrição</span><span class="sxs-lookup"><span data-stu-id="e86e8-140">description</span></span>|<span data-ttu-id="e86e8-141">String</span><span class="sxs-lookup"><span data-stu-id="e86e8-141">String</span></span>|<span data-ttu-id="e86e8-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e86e8-142">The description of the app.</span></span> <span data-ttu-id="e86e8-143">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e86e8-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e86e8-144">publicador</span><span class="sxs-lookup"><span data-stu-id="e86e8-144">publisher</span></span>|<span data-ttu-id="e86e8-145">String</span><span class="sxs-lookup"><span data-stu-id="e86e8-145">String</span></span>|<span data-ttu-id="e86e8-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e86e8-146">The publisher of the app.</span></span> <span data-ttu-id="e86e8-147">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e86e8-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e86e8-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e86e8-148">largeIcon</span></span>|[<span data-ttu-id="e86e8-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e86e8-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e86e8-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="e86e8-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="e86e8-151">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e86e8-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e86e8-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e86e8-152">createdDateTime</span></span>|<span data-ttu-id="e86e8-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e86e8-153">DateTimeOffset</span></span>|<span data-ttu-id="e86e8-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e86e8-154">The date and time the app was created.</span></span> <span data-ttu-id="e86e8-155">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e86e8-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e86e8-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e86e8-156">lastModifiedDateTime</span></span>|<span data-ttu-id="e86e8-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e86e8-157">DateTimeOffset</span></span>|<span data-ttu-id="e86e8-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="e86e8-158">The date and time the app was last modified.</span></span> <span data-ttu-id="e86e8-159">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e86e8-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e86e8-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e86e8-160">isFeatured</span></span>|<span data-ttu-id="e86e8-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="e86e8-161">Boolean</span></span>|<span data-ttu-id="e86e8-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e86e8-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e86e8-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e86e8-163">privacyInformationUrl</span></span>|<span data-ttu-id="e86e8-164">String</span><span class="sxs-lookup"><span data-stu-id="e86e8-164">String</span></span>|<span data-ttu-id="e86e8-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="e86e8-165">The privacy statement Url.</span></span> <span data-ttu-id="e86e8-166">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e86e8-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e86e8-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e86e8-167">informationUrl</span></span>|<span data-ttu-id="e86e8-168">String</span><span class="sxs-lookup"><span data-stu-id="e86e8-168">String</span></span>|<span data-ttu-id="e86e8-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="e86e8-169">The more information Url.</span></span> <span data-ttu-id="e86e8-170">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e86e8-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e86e8-171">owner</span><span class="sxs-lookup"><span data-stu-id="e86e8-171">owner</span></span>|<span data-ttu-id="e86e8-172">String</span><span class="sxs-lookup"><span data-stu-id="e86e8-172">String</span></span>|<span data-ttu-id="e86e8-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="e86e8-173">The owner of the app.</span></span> <span data-ttu-id="e86e8-174">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e86e8-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e86e8-175">developer</span><span class="sxs-lookup"><span data-stu-id="e86e8-175">developer</span></span>|<span data-ttu-id="e86e8-176">String</span><span class="sxs-lookup"><span data-stu-id="e86e8-176">String</span></span>|<span data-ttu-id="e86e8-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e86e8-177">The developer of the app.</span></span> <span data-ttu-id="e86e8-178">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e86e8-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e86e8-179">notes</span><span class="sxs-lookup"><span data-stu-id="e86e8-179">notes</span></span>|<span data-ttu-id="e86e8-180">String</span><span class="sxs-lookup"><span data-stu-id="e86e8-180">String</span></span>|<span data-ttu-id="e86e8-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e86e8-181">Notes for the app.</span></span> <span data-ttu-id="e86e8-182">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e86e8-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e86e8-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="e86e8-183">uploadState</span></span>|<span data-ttu-id="e86e8-184">Int32</span><span class="sxs-lookup"><span data-stu-id="e86e8-184">Int32</span></span>|<span data-ttu-id="e86e8-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="e86e8-185">The upload state.</span></span> <span data-ttu-id="e86e8-186">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e86e8-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e86e8-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="e86e8-187">publishingState</span></span>|[<span data-ttu-id="e86e8-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="e86e8-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="e86e8-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e86e8-189">The publishing state for the app.</span></span> <span data-ttu-id="e86e8-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="e86e8-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="e86e8-191">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e86e8-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="e86e8-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="e86e8-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="e86e8-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="e86e8-193">isAssigned</span></span>|<span data-ttu-id="e86e8-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="e86e8-194">Boolean</span></span>|<span data-ttu-id="e86e8-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="e86e8-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="e86e8-196">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e86e8-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e86e8-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e86e8-197">roleScopeTagIds</span></span>|<span data-ttu-id="e86e8-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e86e8-198">String collection</span></span>|<span data-ttu-id="e86e8-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="e86e8-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="e86e8-200">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e86e8-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e86e8-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="e86e8-201">dependentAppCount</span></span>|<span data-ttu-id="e86e8-202">Int32</span><span class="sxs-lookup"><span data-stu-id="e86e8-202">Int32</span></span>|<span data-ttu-id="e86e8-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="e86e8-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="e86e8-204">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e86e8-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e86e8-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="e86e8-205">committedContentVersion</span></span>|<span data-ttu-id="e86e8-206">String</span><span class="sxs-lookup"><span data-stu-id="e86e8-206">String</span></span>|<span data-ttu-id="e86e8-207">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="e86e8-207">The internal committed content version.</span></span> <span data-ttu-id="e86e8-208">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="e86e8-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e86e8-209">fileName</span><span class="sxs-lookup"><span data-stu-id="e86e8-209">fileName</span></span>|<span data-ttu-id="e86e8-210">String</span><span class="sxs-lookup"><span data-stu-id="e86e8-210">String</span></span>|<span data-ttu-id="e86e8-211">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="e86e8-211">The name of the main Lob application file.</span></span> <span data-ttu-id="e86e8-212">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="e86e8-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e86e8-213">size</span><span class="sxs-lookup"><span data-stu-id="e86e8-213">size</span></span>|<span data-ttu-id="e86e8-214">Int64</span><span class="sxs-lookup"><span data-stu-id="e86e8-214">Int64</span></span>|<span data-ttu-id="e86e8-215">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="e86e8-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="e86e8-216">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="e86e8-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e86e8-217">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="e86e8-217">applicableArchitectures</span></span>|[<span data-ttu-id="e86e8-218">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="e86e8-218">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="e86e8-219">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="e86e8-219">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="e86e8-220">Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="e86e8-220">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="e86e8-221">applicableDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="e86e8-221">applicableDeviceTypes</span></span>|[<span data-ttu-id="e86e8-222">windowsDeviceType</span><span class="sxs-lookup"><span data-stu-id="e86e8-222">windowsDeviceType</span></span>](../resources/intune-apps-windowsdevicetype.md)|<span data-ttu-id="e86e8-223">Os tipos de dispositivos Windows nos quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="e86e8-223">The Windows device type(s) for which this app can run on.</span></span> <span data-ttu-id="e86e8-224">Os valores possíveis são: `none`, `desktop`, `mobile`, `holographic`, `team`.</span><span class="sxs-lookup"><span data-stu-id="e86e8-224">Possible values are: `none`, `desktop`, `mobile`, `holographic`, `team`.</span></span>|
|<span data-ttu-id="e86e8-225">identityName</span><span class="sxs-lookup"><span data-stu-id="e86e8-225">identityName</span></span>|<span data-ttu-id="e86e8-226">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e86e8-226">String</span></span>|<span data-ttu-id="e86e8-227">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="e86e8-227">The Identity Name.</span></span>|
|<span data-ttu-id="e86e8-228">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="e86e8-228">identityPublisherHash</span></span>|<span data-ttu-id="e86e8-229">String</span><span class="sxs-lookup"><span data-stu-id="e86e8-229">String</span></span>|<span data-ttu-id="e86e8-230">O Hash do Publicador de Identidade.</span><span class="sxs-lookup"><span data-stu-id="e86e8-230">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="e86e8-231">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="e86e8-231">identityResourceIdentifier</span></span>|<span data-ttu-id="e86e8-232">String</span><span class="sxs-lookup"><span data-stu-id="e86e8-232">String</span></span>|<span data-ttu-id="e86e8-233">O Identificador de Recurso da Identidade.</span><span class="sxs-lookup"><span data-stu-id="e86e8-233">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="e86e8-234">isBundle</span><span class="sxs-lookup"><span data-stu-id="e86e8-234">isBundle</span></span>|<span data-ttu-id="e86e8-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="e86e8-235">Boolean</span></span>|<span data-ttu-id="e86e8-236">Se o aplicativo é um pacote ou não.</span><span class="sxs-lookup"><span data-stu-id="e86e8-236">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="e86e8-237">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e86e8-237">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="e86e8-238">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e86e8-238">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="e86e8-239">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="e86e8-239">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="e86e8-240">identityVersion</span><span class="sxs-lookup"><span data-stu-id="e86e8-240">identityVersion</span></span>|<span data-ttu-id="e86e8-241">String</span><span class="sxs-lookup"><span data-stu-id="e86e8-241">String</span></span>|<span data-ttu-id="e86e8-242">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="e86e8-242">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="e86e8-243">Resposta</span><span class="sxs-lookup"><span data-stu-id="e86e8-243">Response</span></span>
<span data-ttu-id="e86e8-244">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e86e8-244">If successful, this method returns a `200 OK` response code and an updated [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e86e8-245">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e86e8-245">Example</span></span>

### <a name="request"></a><span data-ttu-id="e86e8-246">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e86e8-246">Request</span></span>
<span data-ttu-id="e86e8-247">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e86e8-247">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1461

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppX",
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
  "applicableArchitectures": "x86",
  "applicableDeviceTypes": "desktop",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true,
    "v10_1809": true,
    "v10_1903": true
  },
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="e86e8-248">Resposta</span><span class="sxs-lookup"><span data-stu-id="e86e8-248">Response</span></span>
<span data-ttu-id="e86e8-p124">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e86e8-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1633

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppX",
  "id": "4bc47eba-7eba-4bc4-ba7e-c44bba7ec44b",
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
  "applicableArchitectures": "x86",
  "applicableDeviceTypes": "desktop",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true,
    "v10_1809": true,
    "v10_1903": true
  },
  "identityVersion": "Identity Version value"
}
```




