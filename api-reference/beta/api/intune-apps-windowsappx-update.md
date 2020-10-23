---
title: Atualizar windowsAppX
description: Atualiza as propriedades de um objeto windowsAppX.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 27a706ec4939215dcefab8061b22d92b1bff7da2
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48709723"
---
# <a name="update-windowsappx"></a><span data-ttu-id="fb85d-103">Atualizar windowsAppX</span><span class="sxs-lookup"><span data-stu-id="fb85d-103">Update windowsAppX</span></span>

<span data-ttu-id="fb85d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb85d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fb85d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fb85d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fb85d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fb85d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb85d-107">Atualiza as propriedades de um objeto [windowsAppX](../resources/intune-apps-windowsappx.md) .</span><span class="sxs-lookup"><span data-stu-id="fb85d-107">Update the properties of a [windowsAppX](../resources/intune-apps-windowsappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fb85d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fb85d-108">Prerequisites</span></span>
<span data-ttu-id="fb85d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb85d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb85d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fb85d-111">Permission type</span></span>|<span data-ttu-id="fb85d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fb85d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb85d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fb85d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fb85d-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb85d-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fb85d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fb85d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb85d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fb85d-116">Not supported.</span></span>|
|<span data-ttu-id="fb85d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fb85d-117">Application</span></span>|<span data-ttu-id="fb85d-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb85d-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb85d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fb85d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="fb85d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fb85d-120">Request headers</span></span>
|<span data-ttu-id="fb85d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fb85d-121">Header</span></span>|<span data-ttu-id="fb85d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="fb85d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb85d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fb85d-123">Authorization</span></span>|<span data-ttu-id="fb85d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fb85d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb85d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fb85d-125">Accept</span></span>|<span data-ttu-id="fb85d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fb85d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb85d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fb85d-127">Request body</span></span>
<span data-ttu-id="fb85d-128">No corpo da solicitação, forneça uma representação JSON do objeto [windowsAppX](../resources/intune-apps-windowsappx.md) .</span><span class="sxs-lookup"><span data-stu-id="fb85d-128">In the request body, supply a JSON representation for the [windowsAppX](../resources/intune-apps-windowsappx.md) object.</span></span>

<span data-ttu-id="fb85d-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsAppX](../resources/intune-apps-windowsappx.md).</span><span class="sxs-lookup"><span data-stu-id="fb85d-129">The following table shows the properties that are required when you create the [windowsAppX](../resources/intune-apps-windowsappx.md).</span></span>

|<span data-ttu-id="fb85d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fb85d-130">Property</span></span>|<span data-ttu-id="fb85d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="fb85d-131">Type</span></span>|<span data-ttu-id="fb85d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb85d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb85d-133">id</span><span class="sxs-lookup"><span data-stu-id="fb85d-133">id</span></span>|<span data-ttu-id="fb85d-134">String</span><span class="sxs-lookup"><span data-stu-id="fb85d-134">String</span></span>|<span data-ttu-id="fb85d-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="fb85d-135">Key of the entity.</span></span> <span data-ttu-id="fb85d-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fb85d-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fb85d-137">displayName</span><span class="sxs-lookup"><span data-stu-id="fb85d-137">displayName</span></span>|<span data-ttu-id="fb85d-138">String</span><span class="sxs-lookup"><span data-stu-id="fb85d-138">String</span></span>|<span data-ttu-id="fb85d-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="fb85d-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="fb85d-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fb85d-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fb85d-141">description</span><span class="sxs-lookup"><span data-stu-id="fb85d-141">description</span></span>|<span data-ttu-id="fb85d-142">String</span><span class="sxs-lookup"><span data-stu-id="fb85d-142">String</span></span>|<span data-ttu-id="fb85d-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fb85d-143">The description of the app.</span></span> <span data-ttu-id="fb85d-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fb85d-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fb85d-145">publicador</span><span class="sxs-lookup"><span data-stu-id="fb85d-145">publisher</span></span>|<span data-ttu-id="fb85d-146">String</span><span class="sxs-lookup"><span data-stu-id="fb85d-146">String</span></span>|<span data-ttu-id="fb85d-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fb85d-147">The publisher of the app.</span></span> <span data-ttu-id="fb85d-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fb85d-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fb85d-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="fb85d-149">largeIcon</span></span>|[<span data-ttu-id="fb85d-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="fb85d-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="fb85d-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="fb85d-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="fb85d-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fb85d-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fb85d-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fb85d-153">createdDateTime</span></span>|<span data-ttu-id="fb85d-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb85d-154">DateTimeOffset</span></span>|<span data-ttu-id="fb85d-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fb85d-155">The date and time the app was created.</span></span> <span data-ttu-id="fb85d-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fb85d-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fb85d-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fb85d-157">lastModifiedDateTime</span></span>|<span data-ttu-id="fb85d-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb85d-158">DateTimeOffset</span></span>|<span data-ttu-id="fb85d-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="fb85d-159">The date and time the app was last modified.</span></span> <span data-ttu-id="fb85d-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fb85d-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fb85d-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="fb85d-161">isFeatured</span></span>|<span data-ttu-id="fb85d-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb85d-162">Boolean</span></span>|<span data-ttu-id="fb85d-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fb85d-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fb85d-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="fb85d-164">privacyInformationUrl</span></span>|<span data-ttu-id="fb85d-165">String</span><span class="sxs-lookup"><span data-stu-id="fb85d-165">String</span></span>|<span data-ttu-id="fb85d-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="fb85d-166">The privacy statement Url.</span></span> <span data-ttu-id="fb85d-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fb85d-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fb85d-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="fb85d-168">informationUrl</span></span>|<span data-ttu-id="fb85d-169">String</span><span class="sxs-lookup"><span data-stu-id="fb85d-169">String</span></span>|<span data-ttu-id="fb85d-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="fb85d-170">The more information Url.</span></span> <span data-ttu-id="fb85d-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fb85d-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fb85d-172">owner</span><span class="sxs-lookup"><span data-stu-id="fb85d-172">owner</span></span>|<span data-ttu-id="fb85d-173">String</span><span class="sxs-lookup"><span data-stu-id="fb85d-173">String</span></span>|<span data-ttu-id="fb85d-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="fb85d-174">The owner of the app.</span></span> <span data-ttu-id="fb85d-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fb85d-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fb85d-176">developer</span><span class="sxs-lookup"><span data-stu-id="fb85d-176">developer</span></span>|<span data-ttu-id="fb85d-177">String</span><span class="sxs-lookup"><span data-stu-id="fb85d-177">String</span></span>|<span data-ttu-id="fb85d-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fb85d-178">The developer of the app.</span></span> <span data-ttu-id="fb85d-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fb85d-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fb85d-180">notes</span><span class="sxs-lookup"><span data-stu-id="fb85d-180">notes</span></span>|<span data-ttu-id="fb85d-181">String</span><span class="sxs-lookup"><span data-stu-id="fb85d-181">String</span></span>|<span data-ttu-id="fb85d-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fb85d-182">Notes for the app.</span></span> <span data-ttu-id="fb85d-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fb85d-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fb85d-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="fb85d-184">uploadState</span></span>|<span data-ttu-id="fb85d-185">Int32</span><span class="sxs-lookup"><span data-stu-id="fb85d-185">Int32</span></span>|<span data-ttu-id="fb85d-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="fb85d-186">The upload state.</span></span> <span data-ttu-id="fb85d-187">Os valores possíveis são: 0- `Not Ready` , 1- `Ready` , 2- `Processing` .</span><span class="sxs-lookup"><span data-stu-id="fb85d-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="fb85d-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fb85d-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fb85d-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="fb85d-189">publishingState</span></span>|[<span data-ttu-id="fb85d-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="fb85d-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="fb85d-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fb85d-191">The publishing state for the app.</span></span> <span data-ttu-id="fb85d-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="fb85d-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="fb85d-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fb85d-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="fb85d-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="fb85d-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="fb85d-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="fb85d-195">isAssigned</span></span>|<span data-ttu-id="fb85d-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb85d-196">Boolean</span></span>|<span data-ttu-id="fb85d-197">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="fb85d-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="fb85d-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fb85d-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fb85d-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fb85d-199">roleScopeTagIds</span></span>|<span data-ttu-id="fb85d-200">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="fb85d-200">String collection</span></span>|<span data-ttu-id="fb85d-201">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="fb85d-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="fb85d-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fb85d-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fb85d-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="fb85d-203">dependentAppCount</span></span>|<span data-ttu-id="fb85d-204">Int32</span><span class="sxs-lookup"><span data-stu-id="fb85d-204">Int32</span></span>|<span data-ttu-id="fb85d-205">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="fb85d-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="fb85d-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fb85d-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fb85d-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="fb85d-207">supersedingAppCount</span></span>|<span data-ttu-id="fb85d-208">Int32</span><span class="sxs-lookup"><span data-stu-id="fb85d-208">Int32</span></span>|<span data-ttu-id="fb85d-209">O número total de aplicativos que este aplicativo substitui direta ou indiretamente.</span><span class="sxs-lookup"><span data-stu-id="fb85d-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="fb85d-210">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fb85d-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fb85d-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="fb85d-211">supersededAppCount</span></span>|<span data-ttu-id="fb85d-212">Int32</span><span class="sxs-lookup"><span data-stu-id="fb85d-212">Int32</span></span>|<span data-ttu-id="fb85d-213">O número total de aplicativos que este aplicativo está substituindo direta ou indiretamente por.</span><span class="sxs-lookup"><span data-stu-id="fb85d-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="fb85d-214">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fb85d-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fb85d-215">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="fb85d-215">committedContentVersion</span></span>|<span data-ttu-id="fb85d-216">String</span><span class="sxs-lookup"><span data-stu-id="fb85d-216">String</span></span>|<span data-ttu-id="fb85d-217">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="fb85d-217">The internal committed content version.</span></span> <span data-ttu-id="fb85d-218">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="fb85d-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="fb85d-219">fileName</span><span class="sxs-lookup"><span data-stu-id="fb85d-219">fileName</span></span>|<span data-ttu-id="fb85d-220">String</span><span class="sxs-lookup"><span data-stu-id="fb85d-220">String</span></span>|<span data-ttu-id="fb85d-221">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="fb85d-221">The name of the main Lob application file.</span></span> <span data-ttu-id="fb85d-222">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="fb85d-222">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="fb85d-223">size</span><span class="sxs-lookup"><span data-stu-id="fb85d-223">size</span></span>|<span data-ttu-id="fb85d-224">Int64</span><span class="sxs-lookup"><span data-stu-id="fb85d-224">Int64</span></span>|<span data-ttu-id="fb85d-225">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="fb85d-225">The total size, including all uploaded files.</span></span> <span data-ttu-id="fb85d-226">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="fb85d-226">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="fb85d-227">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="fb85d-227">applicableArchitectures</span></span>|[<span data-ttu-id="fb85d-228">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="fb85d-228">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="fb85d-229">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="fb85d-229">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="fb85d-230">Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="fb85d-230">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="fb85d-231">identityName</span><span class="sxs-lookup"><span data-stu-id="fb85d-231">identityName</span></span>|<span data-ttu-id="fb85d-232">String</span><span class="sxs-lookup"><span data-stu-id="fb85d-232">String</span></span>|<span data-ttu-id="fb85d-233">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="fb85d-233">The Identity Name.</span></span>|
|<span data-ttu-id="fb85d-234">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="fb85d-234">identityPublisherHash</span></span>|<span data-ttu-id="fb85d-235">String</span><span class="sxs-lookup"><span data-stu-id="fb85d-235">String</span></span>|<span data-ttu-id="fb85d-236">O Hash do Publicador de Identidade.</span><span class="sxs-lookup"><span data-stu-id="fb85d-236">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="fb85d-237">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="fb85d-237">identityResourceIdentifier</span></span>|<span data-ttu-id="fb85d-238">String</span><span class="sxs-lookup"><span data-stu-id="fb85d-238">String</span></span>|<span data-ttu-id="fb85d-239">O Identificador de Recurso da Identidade.</span><span class="sxs-lookup"><span data-stu-id="fb85d-239">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="fb85d-240">isBundle</span><span class="sxs-lookup"><span data-stu-id="fb85d-240">isBundle</span></span>|<span data-ttu-id="fb85d-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb85d-241">Boolean</span></span>|<span data-ttu-id="fb85d-242">Se o aplicativo é um pacote ou não.</span><span class="sxs-lookup"><span data-stu-id="fb85d-242">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="fb85d-243">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="fb85d-243">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="fb85d-244">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="fb85d-244">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="fb85d-245">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="fb85d-245">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="fb85d-246">identityVersion</span><span class="sxs-lookup"><span data-stu-id="fb85d-246">identityVersion</span></span>|<span data-ttu-id="fb85d-247">String</span><span class="sxs-lookup"><span data-stu-id="fb85d-247">String</span></span>|<span data-ttu-id="fb85d-248">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="fb85d-248">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="fb85d-249">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb85d-249">Response</span></span>
<span data-ttu-id="fb85d-250">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [windowsAppX](../resources/intune-apps-windowsappx.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fb85d-250">If successful, this method returns a `200 OK` response code and an updated [windowsAppX](../resources/intune-apps-windowsappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb85d-251">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fb85d-251">Example</span></span>

### <a name="request"></a><span data-ttu-id="fb85d-252">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fb85d-252">Request</span></span>
<span data-ttu-id="fb85d-253">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fb85d-253">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1470

{
  "@odata.type": "#microsoft.graph.windowsAppX",
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
  "applicableArchitectures": "x86",
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

### <a name="response"></a><span data-ttu-id="fb85d-254">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb85d-254">Response</span></span>
<span data-ttu-id="fb85d-p125">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fb85d-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1642

{
  "@odata.type": "#microsoft.graph.windowsAppX",
  "id": "b5179a93-9a93-b517-939a-17b5939a17b5",
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
  "applicableArchitectures": "x86",
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





