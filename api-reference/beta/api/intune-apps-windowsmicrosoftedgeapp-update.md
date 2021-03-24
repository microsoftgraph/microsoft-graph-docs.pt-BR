---
title: Atualizar windowsMicrosoftEdgeApp
description: Atualize as propriedades de um objeto windowsMicrosoftEdgeApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ae11ee91b93ec29f53ba02a933207e55ebc40a59
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51142811"
---
# <a name="update-windowsmicrosoftedgeapp"></a><span data-ttu-id="7f98a-103">Atualizar windowsMicrosoftEdgeApp</span><span class="sxs-lookup"><span data-stu-id="7f98a-103">Update windowsMicrosoftEdgeApp</span></span>

<span data-ttu-id="7f98a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f98a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7f98a-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7f98a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7f98a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7f98a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f98a-107">Atualize as propriedades de um [objeto windowsMicrosoftEdgeApp.](../resources/intune-apps-windowsmicrosoftedgeapp.md)</span><span class="sxs-lookup"><span data-stu-id="7f98a-107">Update the properties of a [windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7f98a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7f98a-108">Prerequisites</span></span>
<span data-ttu-id="7f98a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f98a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f98a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7f98a-111">Permission type</span></span>|<span data-ttu-id="7f98a-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7f98a-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f98a-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7f98a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7f98a-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f98a-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7f98a-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7f98a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f98a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7f98a-116">Not supported.</span></span>|
|<span data-ttu-id="7f98a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7f98a-117">Application</span></span>|<span data-ttu-id="7f98a-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f98a-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f98a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7f98a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="7f98a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7f98a-120">Request headers</span></span>
|<span data-ttu-id="7f98a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7f98a-121">Header</span></span>|<span data-ttu-id="7f98a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7f98a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f98a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7f98a-123">Authorization</span></span>|<span data-ttu-id="7f98a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7f98a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f98a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7f98a-125">Accept</span></span>|<span data-ttu-id="7f98a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7f98a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f98a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7f98a-127">Request body</span></span>
<span data-ttu-id="7f98a-128">No corpo da solicitação, fornece uma representação JSON para o [objeto windowsMicrosoftEdgeApp.](../resources/intune-apps-windowsmicrosoftedgeapp.md)</span><span class="sxs-lookup"><span data-stu-id="7f98a-128">In the request body, supply a JSON representation for the [windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md) object.</span></span>

<span data-ttu-id="7f98a-129">A tabela a seguir mostra as propriedades necessárias ao criar [o windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md).</span><span class="sxs-lookup"><span data-stu-id="7f98a-129">The following table shows the properties that are required when you create the [windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md).</span></span>

|<span data-ttu-id="7f98a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7f98a-130">Property</span></span>|<span data-ttu-id="7f98a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="7f98a-131">Type</span></span>|<span data-ttu-id="7f98a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f98a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f98a-133">id</span><span class="sxs-lookup"><span data-stu-id="7f98a-133">id</span></span>|<span data-ttu-id="7f98a-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7f98a-134">String</span></span>|<span data-ttu-id="7f98a-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="7f98a-135">Key of the entity.</span></span> <span data-ttu-id="7f98a-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7f98a-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7f98a-137">displayName</span><span class="sxs-lookup"><span data-stu-id="7f98a-137">displayName</span></span>|<span data-ttu-id="7f98a-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7f98a-138">String</span></span>|<span data-ttu-id="7f98a-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="7f98a-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="7f98a-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7f98a-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7f98a-141">descrição</span><span class="sxs-lookup"><span data-stu-id="7f98a-141">description</span></span>|<span data-ttu-id="7f98a-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7f98a-142">String</span></span>|<span data-ttu-id="7f98a-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7f98a-143">The description of the app.</span></span> <span data-ttu-id="7f98a-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7f98a-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7f98a-145">publicador</span><span class="sxs-lookup"><span data-stu-id="7f98a-145">publisher</span></span>|<span data-ttu-id="7f98a-146">String</span><span class="sxs-lookup"><span data-stu-id="7f98a-146">String</span></span>|<span data-ttu-id="7f98a-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7f98a-147">The publisher of the app.</span></span> <span data-ttu-id="7f98a-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7f98a-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7f98a-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="7f98a-149">largeIcon</span></span>|[<span data-ttu-id="7f98a-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="7f98a-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="7f98a-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="7f98a-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="7f98a-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7f98a-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7f98a-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7f98a-153">createdDateTime</span></span>|<span data-ttu-id="7f98a-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f98a-154">DateTimeOffset</span></span>|<span data-ttu-id="7f98a-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7f98a-155">The date and time the app was created.</span></span> <span data-ttu-id="7f98a-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7f98a-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7f98a-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7f98a-157">lastModifiedDateTime</span></span>|<span data-ttu-id="7f98a-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f98a-158">DateTimeOffset</span></span>|<span data-ttu-id="7f98a-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="7f98a-159">The date and time the app was last modified.</span></span> <span data-ttu-id="7f98a-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7f98a-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7f98a-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="7f98a-161">isFeatured</span></span>|<span data-ttu-id="7f98a-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f98a-162">Boolean</span></span>|<span data-ttu-id="7f98a-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7f98a-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7f98a-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="7f98a-164">privacyInformationUrl</span></span>|<span data-ttu-id="7f98a-165">String</span><span class="sxs-lookup"><span data-stu-id="7f98a-165">String</span></span>|<span data-ttu-id="7f98a-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="7f98a-166">The privacy statement Url.</span></span> <span data-ttu-id="7f98a-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7f98a-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7f98a-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="7f98a-168">informationUrl</span></span>|<span data-ttu-id="7f98a-169">String</span><span class="sxs-lookup"><span data-stu-id="7f98a-169">String</span></span>|<span data-ttu-id="7f98a-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="7f98a-170">The more information Url.</span></span> <span data-ttu-id="7f98a-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7f98a-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7f98a-172">owner</span><span class="sxs-lookup"><span data-stu-id="7f98a-172">owner</span></span>|<span data-ttu-id="7f98a-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7f98a-173">String</span></span>|<span data-ttu-id="7f98a-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="7f98a-174">The owner of the app.</span></span> <span data-ttu-id="7f98a-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7f98a-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7f98a-176">developer</span><span class="sxs-lookup"><span data-stu-id="7f98a-176">developer</span></span>|<span data-ttu-id="7f98a-177">String</span><span class="sxs-lookup"><span data-stu-id="7f98a-177">String</span></span>|<span data-ttu-id="7f98a-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7f98a-178">The developer of the app.</span></span> <span data-ttu-id="7f98a-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7f98a-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7f98a-180">notes</span><span class="sxs-lookup"><span data-stu-id="7f98a-180">notes</span></span>|<span data-ttu-id="7f98a-181">String</span><span class="sxs-lookup"><span data-stu-id="7f98a-181">String</span></span>|<span data-ttu-id="7f98a-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7f98a-182">Notes for the app.</span></span> <span data-ttu-id="7f98a-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7f98a-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7f98a-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="7f98a-184">uploadState</span></span>|<span data-ttu-id="7f98a-185">Int32</span><span class="sxs-lookup"><span data-stu-id="7f98a-185">Int32</span></span>|<span data-ttu-id="7f98a-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="7f98a-186">The upload state.</span></span> <span data-ttu-id="7f98a-187">Os valores possíveis são: 0 - `Not Ready` , 1 - `Ready` , 2 - `Processing` .</span><span class="sxs-lookup"><span data-stu-id="7f98a-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="7f98a-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7f98a-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7f98a-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="7f98a-189">publishingState</span></span>|[<span data-ttu-id="7f98a-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="7f98a-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="7f98a-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7f98a-191">The publishing state for the app.</span></span> <span data-ttu-id="7f98a-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="7f98a-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="7f98a-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7f98a-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="7f98a-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="7f98a-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="7f98a-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="7f98a-195">isAssigned</span></span>|<span data-ttu-id="7f98a-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f98a-196">Boolean</span></span>|<span data-ttu-id="7f98a-197">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="7f98a-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="7f98a-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7f98a-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7f98a-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7f98a-199">roleScopeTagIds</span></span>|<span data-ttu-id="7f98a-200">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7f98a-200">String collection</span></span>|<span data-ttu-id="7f98a-201">Lista de ids de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="7f98a-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="7f98a-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7f98a-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7f98a-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="7f98a-203">dependentAppCount</span></span>|<span data-ttu-id="7f98a-204">Int32</span><span class="sxs-lookup"><span data-stu-id="7f98a-204">Int32</span></span>|<span data-ttu-id="7f98a-205">O número total de dependências que o aplicativo filho tem.</span><span class="sxs-lookup"><span data-stu-id="7f98a-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="7f98a-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7f98a-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7f98a-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="7f98a-207">supersedingAppCount</span></span>|<span data-ttu-id="7f98a-208">Int32</span><span class="sxs-lookup"><span data-stu-id="7f98a-208">Int32</span></span>|<span data-ttu-id="7f98a-209">O número total de aplicativos que esse aplicativo sobressede direta ou indiretamente.</span><span class="sxs-lookup"><span data-stu-id="7f98a-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="7f98a-210">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7f98a-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7f98a-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="7f98a-211">supersededAppCount</span></span>|<span data-ttu-id="7f98a-212">Int32</span><span class="sxs-lookup"><span data-stu-id="7f98a-212">Int32</span></span>|<span data-ttu-id="7f98a-213">O número total de aplicativos pelos quais esse aplicativo é, direta ou indiretamente, é suplido.</span><span class="sxs-lookup"><span data-stu-id="7f98a-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="7f98a-214">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7f98a-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7f98a-215">channel</span><span class="sxs-lookup"><span data-stu-id="7f98a-215">channel</span></span>|[<span data-ttu-id="7f98a-216">microsoftEdgeChannel</span><span class="sxs-lookup"><span data-stu-id="7f98a-216">microsoftEdgeChannel</span></span>](../resources/intune-apps-microsoftedgechannel.md)|<span data-ttu-id="7f98a-217">O canal a ser instalado em dispositivos de destino.</span><span class="sxs-lookup"><span data-stu-id="7f98a-217">The channel to install on target devices.</span></span> <span data-ttu-id="7f98a-218">Os valores possíveis são: `dev`, `beta`, `stable`.</span><span class="sxs-lookup"><span data-stu-id="7f98a-218">Possible values are: `dev`, `beta`, `stable`.</span></span>|
|<span data-ttu-id="7f98a-219">displayLanguageLocale</span><span class="sxs-lookup"><span data-stu-id="7f98a-219">displayLanguageLocale</span></span>|<span data-ttu-id="7f98a-220">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7f98a-220">String</span></span>|<span data-ttu-id="7f98a-221">A localidade do idioma a ser usada quando o aplicativo edge exibe texto para o usuário.</span><span class="sxs-lookup"><span data-stu-id="7f98a-221">The language locale to use when the Edge app displays text to the user.</span></span>|



## <a name="response"></a><span data-ttu-id="7f98a-222">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f98a-222">Response</span></span>
<span data-ttu-id="7f98a-223">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7f98a-223">If successful, this method returns a `200 OK` response code and an updated [windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f98a-224">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7f98a-224">Example</span></span>

### <a name="request"></a><span data-ttu-id="7f98a-225">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7f98a-225">Request</span></span>
<span data-ttu-id="7f98a-226">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7f98a-226">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 862

{
  "@odata.type": "#microsoft.graph.windowsMicrosoftEdgeApp",
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
  "channel": "beta",
  "displayLanguageLocale": "Display Language Locale value"
}
```

### <a name="response"></a><span data-ttu-id="7f98a-227">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f98a-227">Response</span></span>
<span data-ttu-id="7f98a-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7f98a-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1034

{
  "@odata.type": "#microsoft.graph.windowsMicrosoftEdgeApp",
  "id": "a4d4a316-a316-a4d4-16a3-d4a416a3d4a4",
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
  "channel": "beta",
  "displayLanguageLocale": "Display Language Locale value"
}
```




