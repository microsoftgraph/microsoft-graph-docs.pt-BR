---
title: Atualizar iosLobApp
description: Atualiza as propriedades de um objeto iosLobApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1224c64734bd74a68c0647790597012e8e56cabf
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49252960"
---
# <a name="update-ioslobapp"></a><span data-ttu-id="12d8f-103">Atualizar iosLobApp</span><span class="sxs-lookup"><span data-stu-id="12d8f-103">Update iosLobApp</span></span>

<span data-ttu-id="12d8f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12d8f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="12d8f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="12d8f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="12d8f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="12d8f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12d8f-107">Atualiza as propriedades de um objeto [iosLobApp](../resources/intune-apps-ioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="12d8f-107">Update the properties of a [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="12d8f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="12d8f-108">Prerequisites</span></span>
<span data-ttu-id="12d8f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12d8f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12d8f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="12d8f-111">Permission type</span></span>|<span data-ttu-id="12d8f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="12d8f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12d8f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="12d8f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="12d8f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12d8f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="12d8f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="12d8f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12d8f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="12d8f-116">Not supported.</span></span>|
|<span data-ttu-id="12d8f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="12d8f-117">Application</span></span>|<span data-ttu-id="12d8f-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12d8f-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="12d8f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="12d8f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="12d8f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="12d8f-120">Request headers</span></span>
|<span data-ttu-id="12d8f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="12d8f-121">Header</span></span>|<span data-ttu-id="12d8f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="12d8f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12d8f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="12d8f-123">Authorization</span></span>|<span data-ttu-id="12d8f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="12d8f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12d8f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="12d8f-125">Accept</span></span>|<span data-ttu-id="12d8f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="12d8f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12d8f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="12d8f-127">Request body</span></span>
<span data-ttu-id="12d8f-128">No corpo da solicitação, forneça uma representação JSON do objeto [iosLobApp](../resources/intune-apps-ioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="12d8f-128">In the request body, supply a JSON representation for the [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

<span data-ttu-id="12d8f-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [iosLobApp.](../resources/intune-apps-ioslobapp.md)</span><span class="sxs-lookup"><span data-stu-id="12d8f-129">The following table shows the properties that are required when you create the [iosLobApp](../resources/intune-apps-ioslobapp.md).</span></span>

|<span data-ttu-id="12d8f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="12d8f-130">Property</span></span>|<span data-ttu-id="12d8f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="12d8f-131">Type</span></span>|<span data-ttu-id="12d8f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="12d8f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12d8f-133">id</span><span class="sxs-lookup"><span data-stu-id="12d8f-133">id</span></span>|<span data-ttu-id="12d8f-134">String</span><span class="sxs-lookup"><span data-stu-id="12d8f-134">String</span></span>|<span data-ttu-id="12d8f-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="12d8f-135">Key of the entity.</span></span> <span data-ttu-id="12d8f-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12d8f-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="12d8f-137">displayName</span><span class="sxs-lookup"><span data-stu-id="12d8f-137">displayName</span></span>|<span data-ttu-id="12d8f-138">String</span><span class="sxs-lookup"><span data-stu-id="12d8f-138">String</span></span>|<span data-ttu-id="12d8f-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="12d8f-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="12d8f-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12d8f-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="12d8f-141">description</span><span class="sxs-lookup"><span data-stu-id="12d8f-141">description</span></span>|<span data-ttu-id="12d8f-142">String</span><span class="sxs-lookup"><span data-stu-id="12d8f-142">String</span></span>|<span data-ttu-id="12d8f-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="12d8f-143">The description of the app.</span></span> <span data-ttu-id="12d8f-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12d8f-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="12d8f-145">publicador</span><span class="sxs-lookup"><span data-stu-id="12d8f-145">publisher</span></span>|<span data-ttu-id="12d8f-146">String</span><span class="sxs-lookup"><span data-stu-id="12d8f-146">String</span></span>|<span data-ttu-id="12d8f-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="12d8f-147">The publisher of the app.</span></span> <span data-ttu-id="12d8f-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12d8f-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="12d8f-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="12d8f-149">largeIcon</span></span>|[<span data-ttu-id="12d8f-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="12d8f-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="12d8f-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="12d8f-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="12d8f-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12d8f-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="12d8f-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="12d8f-153">createdDateTime</span></span>|<span data-ttu-id="12d8f-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12d8f-154">DateTimeOffset</span></span>|<span data-ttu-id="12d8f-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="12d8f-155">The date and time the app was created.</span></span> <span data-ttu-id="12d8f-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12d8f-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="12d8f-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="12d8f-157">lastModifiedDateTime</span></span>|<span data-ttu-id="12d8f-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12d8f-158">DateTimeOffset</span></span>|<span data-ttu-id="12d8f-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="12d8f-159">The date and time the app was last modified.</span></span> <span data-ttu-id="12d8f-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12d8f-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="12d8f-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="12d8f-161">isFeatured</span></span>|<span data-ttu-id="12d8f-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="12d8f-162">Boolean</span></span>|<span data-ttu-id="12d8f-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12d8f-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="12d8f-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="12d8f-164">privacyInformationUrl</span></span>|<span data-ttu-id="12d8f-165">String</span><span class="sxs-lookup"><span data-stu-id="12d8f-165">String</span></span>|<span data-ttu-id="12d8f-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="12d8f-166">The privacy statement Url.</span></span> <span data-ttu-id="12d8f-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12d8f-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="12d8f-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="12d8f-168">informationUrl</span></span>|<span data-ttu-id="12d8f-169">String</span><span class="sxs-lookup"><span data-stu-id="12d8f-169">String</span></span>|<span data-ttu-id="12d8f-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="12d8f-170">The more information Url.</span></span> <span data-ttu-id="12d8f-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12d8f-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="12d8f-172">owner</span><span class="sxs-lookup"><span data-stu-id="12d8f-172">owner</span></span>|<span data-ttu-id="12d8f-173">String</span><span class="sxs-lookup"><span data-stu-id="12d8f-173">String</span></span>|<span data-ttu-id="12d8f-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="12d8f-174">The owner of the app.</span></span> <span data-ttu-id="12d8f-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12d8f-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="12d8f-176">developer</span><span class="sxs-lookup"><span data-stu-id="12d8f-176">developer</span></span>|<span data-ttu-id="12d8f-177">String</span><span class="sxs-lookup"><span data-stu-id="12d8f-177">String</span></span>|<span data-ttu-id="12d8f-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="12d8f-178">The developer of the app.</span></span> <span data-ttu-id="12d8f-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12d8f-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="12d8f-180">notes</span><span class="sxs-lookup"><span data-stu-id="12d8f-180">notes</span></span>|<span data-ttu-id="12d8f-181">String</span><span class="sxs-lookup"><span data-stu-id="12d8f-181">String</span></span>|<span data-ttu-id="12d8f-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="12d8f-182">Notes for the app.</span></span> <span data-ttu-id="12d8f-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12d8f-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="12d8f-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="12d8f-184">uploadState</span></span>|<span data-ttu-id="12d8f-185">Int32</span><span class="sxs-lookup"><span data-stu-id="12d8f-185">Int32</span></span>|<span data-ttu-id="12d8f-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="12d8f-186">The upload state.</span></span> <span data-ttu-id="12d8f-187">Os valores possíveis são: 0- `Not Ready` , 1- `Ready` , 2- `Processing` .</span><span class="sxs-lookup"><span data-stu-id="12d8f-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="12d8f-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12d8f-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="12d8f-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="12d8f-189">publishingState</span></span>|[<span data-ttu-id="12d8f-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="12d8f-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="12d8f-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="12d8f-191">The publishing state for the app.</span></span> <span data-ttu-id="12d8f-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="12d8f-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="12d8f-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="12d8f-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="12d8f-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="12d8f-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="12d8f-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="12d8f-195">isAssigned</span></span>|<span data-ttu-id="12d8f-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="12d8f-196">Boolean</span></span>|<span data-ttu-id="12d8f-197">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="12d8f-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="12d8f-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12d8f-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="12d8f-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="12d8f-199">roleScopeTagIds</span></span>|<span data-ttu-id="12d8f-200">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="12d8f-200">String collection</span></span>|<span data-ttu-id="12d8f-201">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="12d8f-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="12d8f-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12d8f-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="12d8f-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="12d8f-203">dependentAppCount</span></span>|<span data-ttu-id="12d8f-204">Int32</span><span class="sxs-lookup"><span data-stu-id="12d8f-204">Int32</span></span>|<span data-ttu-id="12d8f-205">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="12d8f-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="12d8f-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12d8f-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="12d8f-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="12d8f-207">supersedingAppCount</span></span>|<span data-ttu-id="12d8f-208">Int32</span><span class="sxs-lookup"><span data-stu-id="12d8f-208">Int32</span></span>|<span data-ttu-id="12d8f-209">O número total de aplicativos que este aplicativo substitui direta ou indiretamente.</span><span class="sxs-lookup"><span data-stu-id="12d8f-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="12d8f-210">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12d8f-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="12d8f-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="12d8f-211">supersededAppCount</span></span>|<span data-ttu-id="12d8f-212">Int32</span><span class="sxs-lookup"><span data-stu-id="12d8f-212">Int32</span></span>|<span data-ttu-id="12d8f-213">O número total de aplicativos que este aplicativo está substituindo direta ou indiretamente por.</span><span class="sxs-lookup"><span data-stu-id="12d8f-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="12d8f-214">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="12d8f-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="12d8f-215">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="12d8f-215">committedContentVersion</span></span>|<span data-ttu-id="12d8f-216">String</span><span class="sxs-lookup"><span data-stu-id="12d8f-216">String</span></span>|<span data-ttu-id="12d8f-217">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="12d8f-217">The internal committed content version.</span></span> <span data-ttu-id="12d8f-218">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="12d8f-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="12d8f-219">fileName</span><span class="sxs-lookup"><span data-stu-id="12d8f-219">fileName</span></span>|<span data-ttu-id="12d8f-220">String</span><span class="sxs-lookup"><span data-stu-id="12d8f-220">String</span></span>|<span data-ttu-id="12d8f-221">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="12d8f-221">The name of the main Lob application file.</span></span> <span data-ttu-id="12d8f-222">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="12d8f-222">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="12d8f-223">size</span><span class="sxs-lookup"><span data-stu-id="12d8f-223">size</span></span>|<span data-ttu-id="12d8f-224">Int64</span><span class="sxs-lookup"><span data-stu-id="12d8f-224">Int64</span></span>|<span data-ttu-id="12d8f-225">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="12d8f-225">The total size, including all uploaded files.</span></span> <span data-ttu-id="12d8f-226">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="12d8f-226">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="12d8f-227">bundleId</span><span class="sxs-lookup"><span data-stu-id="12d8f-227">bundleId</span></span>|<span data-ttu-id="12d8f-228">String</span><span class="sxs-lookup"><span data-stu-id="12d8f-228">String</span></span>|<span data-ttu-id="12d8f-229">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="12d8f-229">The Identity Name.</span></span>|
|<span data-ttu-id="12d8f-230">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="12d8f-230">applicableDeviceType</span></span>|[<span data-ttu-id="12d8f-231">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="12d8f-231">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="12d8f-232">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="12d8f-232">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="12d8f-233">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="12d8f-233">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="12d8f-234">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="12d8f-234">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="12d8f-235">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="12d8f-235">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="12d8f-236">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="12d8f-236">expirationDateTime</span></span>|<span data-ttu-id="12d8f-237">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12d8f-237">DateTimeOffset</span></span>|<span data-ttu-id="12d8f-238">O tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="12d8f-238">The expiration time.</span></span>|
|<span data-ttu-id="12d8f-239">versionNumber</span><span class="sxs-lookup"><span data-stu-id="12d8f-239">versionNumber</span></span>|<span data-ttu-id="12d8f-240">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="12d8f-240">String</span></span>|<span data-ttu-id="12d8f-241">O número de versão do aplicativo de Linha de Negócios (LoB) iOS.</span><span class="sxs-lookup"><span data-stu-id="12d8f-241">The version number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="12d8f-242">buildNumber</span><span class="sxs-lookup"><span data-stu-id="12d8f-242">buildNumber</span></span>|<span data-ttu-id="12d8f-243">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="12d8f-243">String</span></span>|<span data-ttu-id="12d8f-244">O número de build do aplicativo de Linha de Negócios (LoB) iOS.</span><span class="sxs-lookup"><span data-stu-id="12d8f-244">The build number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="12d8f-245">identityVersion</span><span class="sxs-lookup"><span data-stu-id="12d8f-245">identityVersion</span></span>|<span data-ttu-id="12d8f-246">String</span><span class="sxs-lookup"><span data-stu-id="12d8f-246">String</span></span>|<span data-ttu-id="12d8f-247">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="12d8f-247">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="12d8f-248">Resposta</span><span class="sxs-lookup"><span data-stu-id="12d8f-248">Response</span></span>
<span data-ttu-id="12d8f-249">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [iosLobApp](../resources/intune-apps-ioslobapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="12d8f-249">If successful, this method returns a `200 OK` response code and an updated [iosLobApp](../resources/intune-apps-ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12d8f-250">Exemplo</span><span class="sxs-lookup"><span data-stu-id="12d8f-250">Example</span></span>

### <a name="request"></a><span data-ttu-id="12d8f-251">Solicitação</span><span class="sxs-lookup"><span data-stu-id="12d8f-251">Request</span></span>
<span data-ttu-id="12d8f-252">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="12d8f-252">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1468

{
  "@odata.type": "#microsoft.graph.iosLobApp",
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
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true,
    "v13_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="12d8f-253">Resposta</span><span class="sxs-lookup"><span data-stu-id="12d8f-253">Response</span></span>
<span data-ttu-id="12d8f-p124">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="12d8f-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1640

{
  "@odata.type": "#microsoft.graph.iosLobApp",
  "id": "b34052ea-52ea-b340-ea52-40b3ea5240b3",
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
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true,
    "v13_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```




