---
title: Atualizar macOSLobApp
description: Atualiza as propriedades de um objeto macOSLobApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 458d6f0a69e4ec52120431bf9b27863fe4741013
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48699930"
---
# <a name="update-macoslobapp"></a><span data-ttu-id="e718f-103">Atualizar macOSLobApp</span><span class="sxs-lookup"><span data-stu-id="e718f-103">Update macOSLobApp</span></span>

<span data-ttu-id="e718f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e718f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e718f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e718f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e718f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e718f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e718f-107">Atualiza as propriedades de um objeto [macOSLobApp](../resources/intune-apps-macoslobapp.md) .</span><span class="sxs-lookup"><span data-stu-id="e718f-107">Update the properties of a [macOSLobApp](../resources/intune-apps-macoslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e718f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e718f-108">Prerequisites</span></span>
<span data-ttu-id="e718f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e718f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e718f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e718f-111">Permission type</span></span>|<span data-ttu-id="e718f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e718f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e718f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e718f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e718f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e718f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e718f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e718f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e718f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e718f-116">Not supported.</span></span>|
|<span data-ttu-id="e718f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e718f-117">Application</span></span>|<span data-ttu-id="e718f-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e718f-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e718f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e718f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="e718f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e718f-120">Request headers</span></span>
|<span data-ttu-id="e718f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e718f-121">Header</span></span>|<span data-ttu-id="e718f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e718f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e718f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e718f-123">Authorization</span></span>|<span data-ttu-id="e718f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e718f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e718f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e718f-125">Accept</span></span>|<span data-ttu-id="e718f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e718f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e718f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e718f-127">Request body</span></span>
<span data-ttu-id="e718f-128">No corpo da solicitação, forneça uma representação JSON do objeto [macOSLobApp](../resources/intune-apps-macoslobapp.md) .</span><span class="sxs-lookup"><span data-stu-id="e718f-128">In the request body, supply a JSON representation for the [macOSLobApp](../resources/intune-apps-macoslobapp.md) object.</span></span>

<span data-ttu-id="e718f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [macOSLobApp](../resources/intune-apps-macoslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="e718f-129">The following table shows the properties that are required when you create the [macOSLobApp](../resources/intune-apps-macoslobapp.md).</span></span>

|<span data-ttu-id="e718f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e718f-130">Property</span></span>|<span data-ttu-id="e718f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e718f-131">Type</span></span>|<span data-ttu-id="e718f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e718f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e718f-133">id</span><span class="sxs-lookup"><span data-stu-id="e718f-133">id</span></span>|<span data-ttu-id="e718f-134">String</span><span class="sxs-lookup"><span data-stu-id="e718f-134">String</span></span>|<span data-ttu-id="e718f-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e718f-135">Key of the entity.</span></span> <span data-ttu-id="e718f-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e718f-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e718f-137">displayName</span><span class="sxs-lookup"><span data-stu-id="e718f-137">displayName</span></span>|<span data-ttu-id="e718f-138">String</span><span class="sxs-lookup"><span data-stu-id="e718f-138">String</span></span>|<span data-ttu-id="e718f-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="e718f-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="e718f-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e718f-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e718f-141">description</span><span class="sxs-lookup"><span data-stu-id="e718f-141">description</span></span>|<span data-ttu-id="e718f-142">String</span><span class="sxs-lookup"><span data-stu-id="e718f-142">String</span></span>|<span data-ttu-id="e718f-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e718f-143">The description of the app.</span></span> <span data-ttu-id="e718f-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e718f-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e718f-145">publicador</span><span class="sxs-lookup"><span data-stu-id="e718f-145">publisher</span></span>|<span data-ttu-id="e718f-146">String</span><span class="sxs-lookup"><span data-stu-id="e718f-146">String</span></span>|<span data-ttu-id="e718f-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e718f-147">The publisher of the app.</span></span> <span data-ttu-id="e718f-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e718f-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e718f-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e718f-149">largeIcon</span></span>|[<span data-ttu-id="e718f-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e718f-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e718f-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="e718f-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="e718f-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e718f-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e718f-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e718f-153">createdDateTime</span></span>|<span data-ttu-id="e718f-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e718f-154">DateTimeOffset</span></span>|<span data-ttu-id="e718f-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e718f-155">The date and time the app was created.</span></span> <span data-ttu-id="e718f-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e718f-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e718f-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e718f-157">lastModifiedDateTime</span></span>|<span data-ttu-id="e718f-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e718f-158">DateTimeOffset</span></span>|<span data-ttu-id="e718f-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="e718f-159">The date and time the app was last modified.</span></span> <span data-ttu-id="e718f-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e718f-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e718f-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e718f-161">isFeatured</span></span>|<span data-ttu-id="e718f-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="e718f-162">Boolean</span></span>|<span data-ttu-id="e718f-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e718f-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e718f-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e718f-164">privacyInformationUrl</span></span>|<span data-ttu-id="e718f-165">String</span><span class="sxs-lookup"><span data-stu-id="e718f-165">String</span></span>|<span data-ttu-id="e718f-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="e718f-166">The privacy statement Url.</span></span> <span data-ttu-id="e718f-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e718f-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e718f-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e718f-168">informationUrl</span></span>|<span data-ttu-id="e718f-169">String</span><span class="sxs-lookup"><span data-stu-id="e718f-169">String</span></span>|<span data-ttu-id="e718f-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="e718f-170">The more information Url.</span></span> <span data-ttu-id="e718f-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e718f-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e718f-172">owner</span><span class="sxs-lookup"><span data-stu-id="e718f-172">owner</span></span>|<span data-ttu-id="e718f-173">String</span><span class="sxs-lookup"><span data-stu-id="e718f-173">String</span></span>|<span data-ttu-id="e718f-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="e718f-174">The owner of the app.</span></span> <span data-ttu-id="e718f-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e718f-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e718f-176">developer</span><span class="sxs-lookup"><span data-stu-id="e718f-176">developer</span></span>|<span data-ttu-id="e718f-177">String</span><span class="sxs-lookup"><span data-stu-id="e718f-177">String</span></span>|<span data-ttu-id="e718f-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e718f-178">The developer of the app.</span></span> <span data-ttu-id="e718f-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e718f-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e718f-180">notes</span><span class="sxs-lookup"><span data-stu-id="e718f-180">notes</span></span>|<span data-ttu-id="e718f-181">String</span><span class="sxs-lookup"><span data-stu-id="e718f-181">String</span></span>|<span data-ttu-id="e718f-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e718f-182">Notes for the app.</span></span> <span data-ttu-id="e718f-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e718f-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e718f-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="e718f-184">uploadState</span></span>|<span data-ttu-id="e718f-185">Int32</span><span class="sxs-lookup"><span data-stu-id="e718f-185">Int32</span></span>|<span data-ttu-id="e718f-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="e718f-186">The upload state.</span></span> <span data-ttu-id="e718f-187">Os valores possíveis são: 0- `Not Ready` , 1- `Ready` , 2- `Processing` .</span><span class="sxs-lookup"><span data-stu-id="e718f-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="e718f-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e718f-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e718f-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="e718f-189">publishingState</span></span>|[<span data-ttu-id="e718f-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="e718f-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="e718f-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e718f-191">The publishing state for the app.</span></span> <span data-ttu-id="e718f-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="e718f-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="e718f-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e718f-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="e718f-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="e718f-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="e718f-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="e718f-195">isAssigned</span></span>|<span data-ttu-id="e718f-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="e718f-196">Boolean</span></span>|<span data-ttu-id="e718f-197">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="e718f-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="e718f-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e718f-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e718f-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e718f-199">roleScopeTagIds</span></span>|<span data-ttu-id="e718f-200">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e718f-200">String collection</span></span>|<span data-ttu-id="e718f-201">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="e718f-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="e718f-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e718f-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e718f-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="e718f-203">dependentAppCount</span></span>|<span data-ttu-id="e718f-204">Int32</span><span class="sxs-lookup"><span data-stu-id="e718f-204">Int32</span></span>|<span data-ttu-id="e718f-205">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="e718f-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="e718f-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e718f-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e718f-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="e718f-207">supersedingAppCount</span></span>|<span data-ttu-id="e718f-208">Int32</span><span class="sxs-lookup"><span data-stu-id="e718f-208">Int32</span></span>|<span data-ttu-id="e718f-209">O número total de aplicativos que este aplicativo substitui direta ou indiretamente.</span><span class="sxs-lookup"><span data-stu-id="e718f-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="e718f-210">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e718f-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e718f-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="e718f-211">supersededAppCount</span></span>|<span data-ttu-id="e718f-212">Int32</span><span class="sxs-lookup"><span data-stu-id="e718f-212">Int32</span></span>|<span data-ttu-id="e718f-213">O número total de aplicativos que este aplicativo está substituindo direta ou indiretamente por.</span><span class="sxs-lookup"><span data-stu-id="e718f-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="e718f-214">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e718f-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e718f-215">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="e718f-215">committedContentVersion</span></span>|<span data-ttu-id="e718f-216">String</span><span class="sxs-lookup"><span data-stu-id="e718f-216">String</span></span>|<span data-ttu-id="e718f-217">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="e718f-217">The internal committed content version.</span></span> <span data-ttu-id="e718f-218">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="e718f-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e718f-219">fileName</span><span class="sxs-lookup"><span data-stu-id="e718f-219">fileName</span></span>|<span data-ttu-id="e718f-220">String</span><span class="sxs-lookup"><span data-stu-id="e718f-220">String</span></span>|<span data-ttu-id="e718f-221">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="e718f-221">The name of the main Lob application file.</span></span> <span data-ttu-id="e718f-222">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="e718f-222">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e718f-223">size</span><span class="sxs-lookup"><span data-stu-id="e718f-223">size</span></span>|<span data-ttu-id="e718f-224">Int64</span><span class="sxs-lookup"><span data-stu-id="e718f-224">Int64</span></span>|<span data-ttu-id="e718f-225">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="e718f-225">The total size, including all uploaded files.</span></span> <span data-ttu-id="e718f-226">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="e718f-226">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e718f-227">bundleId</span><span class="sxs-lookup"><span data-stu-id="e718f-227">bundleId</span></span>|<span data-ttu-id="e718f-228">String</span><span class="sxs-lookup"><span data-stu-id="e718f-228">String</span></span>|<span data-ttu-id="e718f-229">A ID do pacote.</span><span class="sxs-lookup"><span data-stu-id="e718f-229">The bundle id.</span></span>|
|<span data-ttu-id="e718f-230">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e718f-230">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="e718f-231">macOSMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e718f-231">macOSMinimumOperatingSystem</span></span>](../resources/intune-apps-macosminimumoperatingsystem.md)|<span data-ttu-id="e718f-232">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="e718f-232">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="e718f-233">buildNumber</span><span class="sxs-lookup"><span data-stu-id="e718f-233">buildNumber</span></span>|<span data-ttu-id="e718f-234">String</span><span class="sxs-lookup"><span data-stu-id="e718f-234">String</span></span>|<span data-ttu-id="e718f-235">O número de compilação do aplicativo de linha de negócios (LoB) MacOS.</span><span class="sxs-lookup"><span data-stu-id="e718f-235">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="e718f-236">versionNumber</span><span class="sxs-lookup"><span data-stu-id="e718f-236">versionNumber</span></span>|<span data-ttu-id="e718f-237">String</span><span class="sxs-lookup"><span data-stu-id="e718f-237">String</span></span>|<span data-ttu-id="e718f-238">O número da versão do aplicativo de linha de negócios (LoB) MacOS.</span><span class="sxs-lookup"><span data-stu-id="e718f-238">The version number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="e718f-239">childApps</span><span class="sxs-lookup"><span data-stu-id="e718f-239">childApps</span></span>|<span data-ttu-id="e718f-240">coleção [macOSLobChildApp](../resources/intune-apps-macoslobchildapp.md)</span><span class="sxs-lookup"><span data-stu-id="e718f-240">[macOSLobChildApp](../resources/intune-apps-macoslobchildapp.md) collection</span></span>|<span data-ttu-id="e718f-241">A lista de aplicativos neste pacote de pacotes</span><span class="sxs-lookup"><span data-stu-id="e718f-241">The app list in this bundle package</span></span>|
|<span data-ttu-id="e718f-242">identityVersion</span><span class="sxs-lookup"><span data-stu-id="e718f-242">identityVersion</span></span>|<span data-ttu-id="e718f-243">String</span><span class="sxs-lookup"><span data-stu-id="e718f-243">String</span></span>|<span data-ttu-id="e718f-244">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="e718f-244">The identity version.</span></span>|
|<span data-ttu-id="e718f-245">md5HashChunkSize</span><span class="sxs-lookup"><span data-stu-id="e718f-245">md5HashChunkSize</span></span>|<span data-ttu-id="e718f-246">Int32</span><span class="sxs-lookup"><span data-stu-id="e718f-246">Int32</span></span>|<span data-ttu-id="e718f-247">O tamanho da parte do hash MD5</span><span class="sxs-lookup"><span data-stu-id="e718f-247">The chunk size for MD5 hash</span></span>|
|<span data-ttu-id="e718f-248">md5Hash</span><span class="sxs-lookup"><span data-stu-id="e718f-248">md5Hash</span></span>|<span data-ttu-id="e718f-249">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e718f-249">String collection</span></span>|<span data-ttu-id="e718f-250">Os códigos de hash MD5</span><span class="sxs-lookup"><span data-stu-id="e718f-250">The MD5 hash codes</span></span>|
|<span data-ttu-id="e718f-251">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="e718f-251">ignoreVersionDetection</span></span>|<span data-ttu-id="e718f-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="e718f-252">Boolean</span></span>|<span data-ttu-id="e718f-253">Um booliano para controlar se a versão do aplicativo será usada para detectar o aplicativo depois que ele for instalado em um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e718f-253">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="e718f-254">Defina isso como true para aplicativos de linha de negócios (LoB) de macOS que usam um recurso de autoatualização.</span><span class="sxs-lookup"><span data-stu-id="e718f-254">Set this to true for macOS Line of Business (LoB) apps that use a self update feature.</span></span>|
|<span data-ttu-id="e718f-255">installAsManaged</span><span class="sxs-lookup"><span data-stu-id="e718f-255">installAsManaged</span></span>|<span data-ttu-id="e718f-256">Boolean</span><span class="sxs-lookup"><span data-stu-id="e718f-256">Boolean</span></span>|<span data-ttu-id="e718f-257">Um booliano para controlar se o aplicativo será instalado como gerenciado (requer o macOS 11,0 e outras restrições de PKG).</span><span class="sxs-lookup"><span data-stu-id="e718f-257">A boolean to control whether the app will be installed as managed (requires macOS 11.0 and other PKG restrictions).</span></span>|



## <a name="response"></a><span data-ttu-id="e718f-258">Resposta</span><span class="sxs-lookup"><span data-stu-id="e718f-258">Response</span></span>
<span data-ttu-id="e718f-259">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [macOSLobApp](../resources/intune-apps-macoslobapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e718f-259">If successful, this method returns a `200 OK` response code and an updated [macOSLobApp](../resources/intune-apps-macoslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e718f-260">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e718f-260">Example</span></span>

### <a name="request"></a><span data-ttu-id="e718f-261">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e718f-261">Request</span></span>
<span data-ttu-id="e718f-262">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e718f-262">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1702

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
  "supersedingAppCount": 3,
  "supersededAppCount": 2,
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
  "ignoreVersionDetection": true,
  "installAsManaged": true
}
```

### <a name="response"></a><span data-ttu-id="e718f-263">Resposta</span><span class="sxs-lookup"><span data-stu-id="e718f-263">Response</span></span>
<span data-ttu-id="e718f-p125">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e718f-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1874

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
  "supersedingAppCount": 3,
  "supersededAppCount": 2,
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
  "ignoreVersionDetection": true,
  "installAsManaged": true
}
```





