---
title: Atualizar win32LobApp
description: Atualizar as propriedades de um objeto win32LobApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 242341eca66747ed401f177880677bbc5cb017af
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157138"
---
# <a name="update-win32lobapp"></a><span data-ttu-id="30cf0-103">Atualizar win32LobApp</span><span class="sxs-lookup"><span data-stu-id="30cf0-103">Update win32LobApp</span></span>

<span data-ttu-id="30cf0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="30cf0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="30cf0-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="30cf0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="30cf0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="30cf0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30cf0-107">Atualizar as propriedades de um [objeto win32LobApp.](../resources/intune-apps-win32lobapp.md)</span><span class="sxs-lookup"><span data-stu-id="30cf0-107">Update the properties of a [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="30cf0-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="30cf0-108">Prerequisites</span></span>
<span data-ttu-id="30cf0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30cf0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30cf0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="30cf0-111">Permission type</span></span>|<span data-ttu-id="30cf0-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="30cf0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30cf0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="30cf0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="30cf0-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30cf0-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="30cf0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="30cf0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="30cf0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="30cf0-116">Not supported.</span></span>|
|<span data-ttu-id="30cf0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="30cf0-117">Application</span></span>|<span data-ttu-id="30cf0-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30cf0-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="30cf0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="30cf0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="30cf0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="30cf0-120">Request headers</span></span>
|<span data-ttu-id="30cf0-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="30cf0-121">Header</span></span>|<span data-ttu-id="30cf0-122">Valor</span><span class="sxs-lookup"><span data-stu-id="30cf0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="30cf0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="30cf0-123">Authorization</span></span>|<span data-ttu-id="30cf0-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="30cf0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="30cf0-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="30cf0-125">Accept</span></span>|<span data-ttu-id="30cf0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="30cf0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="30cf0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="30cf0-127">Request body</span></span>
<span data-ttu-id="30cf0-128">No corpo da solicitação, fornece uma representação JSON do [objeto win32LobApp.](../resources/intune-apps-win32lobapp.md)</span><span class="sxs-lookup"><span data-stu-id="30cf0-128">In the request body, supply a JSON representation for the [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

<span data-ttu-id="30cf0-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [win32LobApp](../resources/intune-apps-win32lobapp.md).</span><span class="sxs-lookup"><span data-stu-id="30cf0-129">The following table shows the properties that are required when you create the [win32LobApp](../resources/intune-apps-win32lobapp.md).</span></span>

|<span data-ttu-id="30cf0-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="30cf0-130">Property</span></span>|<span data-ttu-id="30cf0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="30cf0-131">Type</span></span>|<span data-ttu-id="30cf0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="30cf0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30cf0-133">id</span><span class="sxs-lookup"><span data-stu-id="30cf0-133">id</span></span>|<span data-ttu-id="30cf0-134">String</span><span class="sxs-lookup"><span data-stu-id="30cf0-134">String</span></span>|<span data-ttu-id="30cf0-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="30cf0-135">Key of the entity.</span></span> <span data-ttu-id="30cf0-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="30cf0-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30cf0-137">displayName</span><span class="sxs-lookup"><span data-stu-id="30cf0-137">displayName</span></span>|<span data-ttu-id="30cf0-138">String</span><span class="sxs-lookup"><span data-stu-id="30cf0-138">String</span></span>|<span data-ttu-id="30cf0-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="30cf0-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="30cf0-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="30cf0-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30cf0-141">description</span><span class="sxs-lookup"><span data-stu-id="30cf0-141">description</span></span>|<span data-ttu-id="30cf0-142">String</span><span class="sxs-lookup"><span data-stu-id="30cf0-142">String</span></span>|<span data-ttu-id="30cf0-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="30cf0-143">The description of the app.</span></span> <span data-ttu-id="30cf0-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="30cf0-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30cf0-145">publicador</span><span class="sxs-lookup"><span data-stu-id="30cf0-145">publisher</span></span>|<span data-ttu-id="30cf0-146">String</span><span class="sxs-lookup"><span data-stu-id="30cf0-146">String</span></span>|<span data-ttu-id="30cf0-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="30cf0-147">The publisher of the app.</span></span> <span data-ttu-id="30cf0-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="30cf0-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30cf0-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="30cf0-149">largeIcon</span></span>|[<span data-ttu-id="30cf0-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="30cf0-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="30cf0-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="30cf0-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="30cf0-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="30cf0-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30cf0-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="30cf0-153">createdDateTime</span></span>|<span data-ttu-id="30cf0-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30cf0-154">DateTimeOffset</span></span>|<span data-ttu-id="30cf0-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="30cf0-155">The date and time the app was created.</span></span> <span data-ttu-id="30cf0-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="30cf0-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30cf0-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="30cf0-157">lastModifiedDateTime</span></span>|<span data-ttu-id="30cf0-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30cf0-158">DateTimeOffset</span></span>|<span data-ttu-id="30cf0-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="30cf0-159">The date and time the app was last modified.</span></span> <span data-ttu-id="30cf0-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="30cf0-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30cf0-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="30cf0-161">isFeatured</span></span>|<span data-ttu-id="30cf0-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="30cf0-162">Boolean</span></span>|<span data-ttu-id="30cf0-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="30cf0-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30cf0-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="30cf0-164">privacyInformationUrl</span></span>|<span data-ttu-id="30cf0-165">String</span><span class="sxs-lookup"><span data-stu-id="30cf0-165">String</span></span>|<span data-ttu-id="30cf0-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="30cf0-166">The privacy statement Url.</span></span> <span data-ttu-id="30cf0-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="30cf0-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30cf0-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="30cf0-168">informationUrl</span></span>|<span data-ttu-id="30cf0-169">String</span><span class="sxs-lookup"><span data-stu-id="30cf0-169">String</span></span>|<span data-ttu-id="30cf0-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="30cf0-170">The more information Url.</span></span> <span data-ttu-id="30cf0-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="30cf0-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30cf0-172">owner</span><span class="sxs-lookup"><span data-stu-id="30cf0-172">owner</span></span>|<span data-ttu-id="30cf0-173">String</span><span class="sxs-lookup"><span data-stu-id="30cf0-173">String</span></span>|<span data-ttu-id="30cf0-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="30cf0-174">The owner of the app.</span></span> <span data-ttu-id="30cf0-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="30cf0-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30cf0-176">developer</span><span class="sxs-lookup"><span data-stu-id="30cf0-176">developer</span></span>|<span data-ttu-id="30cf0-177">String</span><span class="sxs-lookup"><span data-stu-id="30cf0-177">String</span></span>|<span data-ttu-id="30cf0-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="30cf0-178">The developer of the app.</span></span> <span data-ttu-id="30cf0-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="30cf0-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30cf0-180">notes</span><span class="sxs-lookup"><span data-stu-id="30cf0-180">notes</span></span>|<span data-ttu-id="30cf0-181">String</span><span class="sxs-lookup"><span data-stu-id="30cf0-181">String</span></span>|<span data-ttu-id="30cf0-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="30cf0-182">Notes for the app.</span></span> <span data-ttu-id="30cf0-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="30cf0-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30cf0-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="30cf0-184">uploadState</span></span>|<span data-ttu-id="30cf0-185">Int32</span><span class="sxs-lookup"><span data-stu-id="30cf0-185">Int32</span></span>|<span data-ttu-id="30cf0-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="30cf0-186">The upload state.</span></span> <span data-ttu-id="30cf0-187">Os valores possíveis são: 0 - `Not Ready` , 1 - `Ready` , 2 - `Processing` .</span><span class="sxs-lookup"><span data-stu-id="30cf0-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="30cf0-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="30cf0-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30cf0-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="30cf0-189">publishingState</span></span>|[<span data-ttu-id="30cf0-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="30cf0-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="30cf0-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="30cf0-191">The publishing state for the app.</span></span> <span data-ttu-id="30cf0-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="30cf0-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="30cf0-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30cf0-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="30cf0-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="30cf0-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="30cf0-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="30cf0-195">isAssigned</span></span>|<span data-ttu-id="30cf0-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="30cf0-196">Boolean</span></span>|<span data-ttu-id="30cf0-197">O valor que indica se o aplicativo está atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="30cf0-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="30cf0-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="30cf0-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30cf0-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="30cf0-199">roleScopeTagIds</span></span>|<span data-ttu-id="30cf0-200">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="30cf0-200">String collection</span></span>|<span data-ttu-id="30cf0-201">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="30cf0-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="30cf0-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="30cf0-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30cf0-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="30cf0-203">dependentAppCount</span></span>|<span data-ttu-id="30cf0-204">Int32</span><span class="sxs-lookup"><span data-stu-id="30cf0-204">Int32</span></span>|<span data-ttu-id="30cf0-205">O número total de dependências que o aplicativo filho tem.</span><span class="sxs-lookup"><span data-stu-id="30cf0-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="30cf0-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="30cf0-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30cf0-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="30cf0-207">supersedingAppCount</span></span>|<span data-ttu-id="30cf0-208">Int32</span><span class="sxs-lookup"><span data-stu-id="30cf0-208">Int32</span></span>|<span data-ttu-id="30cf0-209">O número total de aplicativos que este aplicativo é direta ou indiretamente é supersedido.</span><span class="sxs-lookup"><span data-stu-id="30cf0-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="30cf0-210">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="30cf0-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30cf0-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="30cf0-211">supersededAppCount</span></span>|<span data-ttu-id="30cf0-212">Int32</span><span class="sxs-lookup"><span data-stu-id="30cf0-212">Int32</span></span>|<span data-ttu-id="30cf0-213">O número total de aplicativos pelos quais esse aplicativo é direta ou indiretamente sobressu valorado.</span><span class="sxs-lookup"><span data-stu-id="30cf0-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="30cf0-214">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="30cf0-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30cf0-215">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="30cf0-215">committedContentVersion</span></span>|<span data-ttu-id="30cf0-216">String</span><span class="sxs-lookup"><span data-stu-id="30cf0-216">String</span></span>|<span data-ttu-id="30cf0-217">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="30cf0-217">The internal committed content version.</span></span> <span data-ttu-id="30cf0-218">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="30cf0-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="30cf0-219">fileName</span><span class="sxs-lookup"><span data-stu-id="30cf0-219">fileName</span></span>|<span data-ttu-id="30cf0-220">String</span><span class="sxs-lookup"><span data-stu-id="30cf0-220">String</span></span>|<span data-ttu-id="30cf0-221">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="30cf0-221">The name of the main Lob application file.</span></span> <span data-ttu-id="30cf0-222">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="30cf0-222">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="30cf0-223">size</span><span class="sxs-lookup"><span data-stu-id="30cf0-223">size</span></span>|<span data-ttu-id="30cf0-224">Int64</span><span class="sxs-lookup"><span data-stu-id="30cf0-224">Int64</span></span>|<span data-ttu-id="30cf0-225">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="30cf0-225">The total size, including all uploaded files.</span></span> <span data-ttu-id="30cf0-226">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="30cf0-226">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="30cf0-227">installCommandLine</span><span class="sxs-lookup"><span data-stu-id="30cf0-227">installCommandLine</span></span>|<span data-ttu-id="30cf0-228">String</span><span class="sxs-lookup"><span data-stu-id="30cf0-228">String</span></span>|<span data-ttu-id="30cf0-229">A linha de comando para instalar este aplicativo</span><span class="sxs-lookup"><span data-stu-id="30cf0-229">The command line to install this app</span></span>|
|<span data-ttu-id="30cf0-230">uninstallCommandLine</span><span class="sxs-lookup"><span data-stu-id="30cf0-230">uninstallCommandLine</span></span>|<span data-ttu-id="30cf0-231">String</span><span class="sxs-lookup"><span data-stu-id="30cf0-231">String</span></span>|<span data-ttu-id="30cf0-232">A linha de comando para desinstalar este aplicativo</span><span class="sxs-lookup"><span data-stu-id="30cf0-232">The command line to uninstall this app</span></span>|
|<span data-ttu-id="30cf0-233">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="30cf0-233">applicableArchitectures</span></span>|[<span data-ttu-id="30cf0-234">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="30cf0-234">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="30cf0-235">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="30cf0-235">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="30cf0-236">Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="30cf0-236">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="30cf0-237">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="30cf0-237">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="30cf0-238">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="30cf0-238">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="30cf0-239">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="30cf0-239">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="30cf0-240">minimumFreeDiskSpaceInMB</span><span class="sxs-lookup"><span data-stu-id="30cf0-240">minimumFreeDiskSpaceInMB</span></span>|<span data-ttu-id="30cf0-241">Int32</span><span class="sxs-lookup"><span data-stu-id="30cf0-241">Int32</span></span>|<span data-ttu-id="30cf0-242">O valor do espaço em disco livre mínimo necessário para instalar esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="30cf0-242">The value for the minimum free disk space which is required to install this app.</span></span>|
|<span data-ttu-id="30cf0-243">minimumMemoryInMB</span><span class="sxs-lookup"><span data-stu-id="30cf0-243">minimumMemoryInMB</span></span>|<span data-ttu-id="30cf0-244">Int32</span><span class="sxs-lookup"><span data-stu-id="30cf0-244">Int32</span></span>|<span data-ttu-id="30cf0-245">O valor da memória física mínima necessária para instalar esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="30cf0-245">The value for the minimum physical memory which is required to install this app.</span></span>|
|<span data-ttu-id="30cf0-246">minimumNumberOfProcessors</span><span class="sxs-lookup"><span data-stu-id="30cf0-246">minimumNumberOfProcessors</span></span>|<span data-ttu-id="30cf0-247">Int32</span><span class="sxs-lookup"><span data-stu-id="30cf0-247">Int32</span></span>|<span data-ttu-id="30cf0-248">O valor do número mínimo de processadores necessário para instalar esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="30cf0-248">The value for the minimum number of processors which is required to install this app.</span></span>|
|<span data-ttu-id="30cf0-249">minimumCpuSpeedInMHz</span><span class="sxs-lookup"><span data-stu-id="30cf0-249">minimumCpuSpeedInMHz</span></span>|<span data-ttu-id="30cf0-250">Int32</span><span class="sxs-lookup"><span data-stu-id="30cf0-250">Int32</span></span>|<span data-ttu-id="30cf0-251">O valor da velocidade mínima da CPU necessária para instalar esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="30cf0-251">The value for the minimum CPU speed which is required to install this app.</span></span>|
|<span data-ttu-id="30cf0-252">detectionRules</span><span class="sxs-lookup"><span data-stu-id="30cf0-252">detectionRules</span></span>|<span data-ttu-id="30cf0-253">[Coleção win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="30cf0-253">[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md) collection</span></span>|<span data-ttu-id="30cf0-254">As regras de detecção para detectar o aplicativo Win32 Line of Business (LoB).</span><span class="sxs-lookup"><span data-stu-id="30cf0-254">The detection rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="30cf0-255">requirementRules</span><span class="sxs-lookup"><span data-stu-id="30cf0-255">requirementRules</span></span>|<span data-ttu-id="30cf0-256">[Coleção win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="30cf0-256">[win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md) collection</span></span>|<span data-ttu-id="30cf0-257">As regras de requisito para detectar o aplicativo Win32 Line of Business (LoB).</span><span class="sxs-lookup"><span data-stu-id="30cf0-257">The requirement rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="30cf0-258">rules</span><span class="sxs-lookup"><span data-stu-id="30cf0-258">rules</span></span>|<span data-ttu-id="30cf0-259">[Coleção win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span><span class="sxs-lookup"><span data-stu-id="30cf0-259">[win32LobAppRule](../resources/intune-apps-win32lobapprule.md) collection</span></span>|<span data-ttu-id="30cf0-260">As regras de detecção e requisitos para este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="30cf0-260">The detection and requirement rules for this app.</span></span>|
|<span data-ttu-id="30cf0-261">installExperience</span><span class="sxs-lookup"><span data-stu-id="30cf0-261">installExperience</span></span>|[<span data-ttu-id="30cf0-262">win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="30cf0-262">win32LobAppInstallExperience</span></span>](../resources/intune-apps-win32lobappinstallexperience.md)|<span data-ttu-id="30cf0-263">A experiência de instalação deste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="30cf0-263">The install experience for this app.</span></span>|
|<span data-ttu-id="30cf0-264">returnCodes</span><span class="sxs-lookup"><span data-stu-id="30cf0-264">returnCodes</span></span>|<span data-ttu-id="30cf0-265">[Coleção win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md)</span><span class="sxs-lookup"><span data-stu-id="30cf0-265">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md) collection</span></span>|<span data-ttu-id="30cf0-266">Os códigos de retorno para o comportamento pós-instalação.</span><span class="sxs-lookup"><span data-stu-id="30cf0-266">The return codes for post installation behavior.</span></span>|
|<span data-ttu-id="30cf0-267">msiInformation</span><span class="sxs-lookup"><span data-stu-id="30cf0-267">msiInformation</span></span>|[<span data-ttu-id="30cf0-268">win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="30cf0-268">win32LobAppMsiInformation</span></span>](../resources/intune-apps-win32lobappmsiinformation.md)|<span data-ttu-id="30cf0-269">Os detalhes do MSI se esse aplicativo Win32 for um aplicativo MSI.</span><span class="sxs-lookup"><span data-stu-id="30cf0-269">The MSI details if this Win32 app is an MSI app.</span></span>|
|<span data-ttu-id="30cf0-270">setupFilePath</span><span class="sxs-lookup"><span data-stu-id="30cf0-270">setupFilePath</span></span>|<span data-ttu-id="30cf0-271">String</span><span class="sxs-lookup"><span data-stu-id="30cf0-271">String</span></span>|<span data-ttu-id="30cf0-272">O caminho relativo do arquivo de instalação no pacote Win32LobApp criptografado.</span><span class="sxs-lookup"><span data-stu-id="30cf0-272">The relative path of the setup file in the encrypted Win32LobApp package.</span></span>|
|<span data-ttu-id="30cf0-273">minimumSupportedWindowsRelease</span><span class="sxs-lookup"><span data-stu-id="30cf0-273">minimumSupportedWindowsRelease</span></span>|<span data-ttu-id="30cf0-274">String</span><span class="sxs-lookup"><span data-stu-id="30cf0-274">String</span></span>|<span data-ttu-id="30cf0-275">O valor da versão mínima do Windows com suporte.</span><span class="sxs-lookup"><span data-stu-id="30cf0-275">The value for the minimum supported windows release.</span></span>|
|<span data-ttu-id="30cf0-276">displayVersion</span><span class="sxs-lookup"><span data-stu-id="30cf0-276">displayVersion</span></span>|<span data-ttu-id="30cf0-277">String</span><span class="sxs-lookup"><span data-stu-id="30cf0-277">String</span></span>|<span data-ttu-id="30cf0-278">A versão exibida na UX desse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="30cf0-278">The version displayed in the UX for this app.</span></span>|



## <a name="response"></a><span data-ttu-id="30cf0-279">Resposta</span><span class="sxs-lookup"><span data-stu-id="30cf0-279">Response</span></span>
<span data-ttu-id="30cf0-280">Se bem-sucedido, este método retorna um código de resposta e um objeto `200 OK` [win32LobApp](../resources/intune-apps-win32lobapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="30cf0-280">If successful, this method returns a `200 OK` response code and an updated [win32LobApp](../resources/intune-apps-win32lobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30cf0-281">Exemplo</span><span class="sxs-lookup"><span data-stu-id="30cf0-281">Example</span></span>

### <a name="request"></a><span data-ttu-id="30cf0-282">Solicitação</span><span class="sxs-lookup"><span data-stu-id="30cf0-282">Request</span></span>
<span data-ttu-id="30cf0-283">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="30cf0-283">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 3405

{
  "@odata.type": "#microsoft.graph.win32LobApp",
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
  "installCommandLine": "Install Command Line value",
  "uninstallCommandLine": "Uninstall Command Line value",
  "applicableArchitectures": "x86",
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
    "v10_1903": true,
    "v10_1909": true,
    "v10_2004": true
  },
  "minimumFreeDiskSpaceInMB": 8,
  "minimumMemoryInMB": 1,
  "minimumNumberOfProcessors": 9,
  "minimumCpuSpeedInMHz": 4,
  "detectionRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryDetection",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists",
      "operator": "equal",
      "detectionValue": "Detection Value value"
    }
  ],
  "requirementRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryRequirement",
      "operator": "equal",
      "detectionValue": "Detection Value value",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists"
    }
  ],
  "rules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryRule",
      "ruleType": "requirement",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "operationType": "exists",
      "operator": "equal",
      "comparisonValue": "Comparison Value value"
    }
  ],
  "installExperience": {
    "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
    "runAsAccount": "user",
    "deviceRestartBehavior": "allow"
  },
  "returnCodes": [
    {
      "@odata.type": "microsoft.graph.win32LobAppReturnCode",
      "returnCode": 10,
      "type": "success"
    }
  ],
  "msiInformation": {
    "@odata.type": "microsoft.graph.win32LobAppMsiInformation",
    "productCode": "Product Code value",
    "productVersion": "Product Version value",
    "upgradeCode": "Upgrade Code value",
    "requiresReboot": true,
    "packageType": "perUser",
    "productName": "Product Name value",
    "publisher": "Publisher value"
  },
  "setupFilePath": "Setup File Path value",
  "minimumSupportedWindowsRelease": "Minimum Supported Windows Release value",
  "displayVersion": "Display Version value"
}
```

### <a name="response"></a><span data-ttu-id="30cf0-284">Resposta</span><span class="sxs-lookup"><span data-stu-id="30cf0-284">Response</span></span>
<span data-ttu-id="30cf0-p125">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="30cf0-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3577

{
  "@odata.type": "#microsoft.graph.win32LobApp",
  "id": "9607b530-b530-9607-30b5-079630b50796",
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
  "installCommandLine": "Install Command Line value",
  "uninstallCommandLine": "Uninstall Command Line value",
  "applicableArchitectures": "x86",
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
    "v10_1903": true,
    "v10_1909": true,
    "v10_2004": true
  },
  "minimumFreeDiskSpaceInMB": 8,
  "minimumMemoryInMB": 1,
  "minimumNumberOfProcessors": 9,
  "minimumCpuSpeedInMHz": 4,
  "detectionRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryDetection",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists",
      "operator": "equal",
      "detectionValue": "Detection Value value"
    }
  ],
  "requirementRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryRequirement",
      "operator": "equal",
      "detectionValue": "Detection Value value",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists"
    }
  ],
  "rules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryRule",
      "ruleType": "requirement",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "operationType": "exists",
      "operator": "equal",
      "comparisonValue": "Comparison Value value"
    }
  ],
  "installExperience": {
    "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
    "runAsAccount": "user",
    "deviceRestartBehavior": "allow"
  },
  "returnCodes": [
    {
      "@odata.type": "microsoft.graph.win32LobAppReturnCode",
      "returnCode": 10,
      "type": "success"
    }
  ],
  "msiInformation": {
    "@odata.type": "microsoft.graph.win32LobAppMsiInformation",
    "productCode": "Product Code value",
    "productVersion": "Product Version value",
    "upgradeCode": "Upgrade Code value",
    "requiresReboot": true,
    "packageType": "perUser",
    "productName": "Product Name value",
    "publisher": "Publisher value"
  },
  "setupFilePath": "Setup File Path value",
  "minimumSupportedWindowsRelease": "Minimum Supported Windows Release value",
  "displayVersion": "Display Version value"
}
```




