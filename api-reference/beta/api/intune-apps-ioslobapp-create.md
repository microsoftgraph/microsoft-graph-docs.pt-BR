---
title: Criar iosLobApp
description: Cria um novo objeto iosLobApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bac65fd7fe3272b6cf52531781271ad22a2068a1
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157411"
---
# <a name="create-ioslobapp"></a><span data-ttu-id="e1174-103">Criar iosLobApp</span><span class="sxs-lookup"><span data-stu-id="e1174-103">Create iosLobApp</span></span>

<span data-ttu-id="e1174-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1174-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e1174-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e1174-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e1174-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e1174-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1174-107">Cria um novo objeto [iosLobApp](../resources/intune-apps-ioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="e1174-107">Create a new [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e1174-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e1174-108">Prerequisites</span></span>
<span data-ttu-id="e1174-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1174-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1174-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e1174-111">Permission type</span></span>|<span data-ttu-id="e1174-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e1174-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1174-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e1174-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e1174-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1174-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e1174-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e1174-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1174-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1174-116">Not supported.</span></span>|
|<span data-ttu-id="e1174-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e1174-117">Application</span></span>|<span data-ttu-id="e1174-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1174-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1174-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e1174-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="e1174-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e1174-120">Request headers</span></span>
|<span data-ttu-id="e1174-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e1174-121">Header</span></span>|<span data-ttu-id="e1174-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e1174-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1174-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e1174-123">Authorization</span></span>|<span data-ttu-id="e1174-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e1174-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1174-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e1174-125">Accept</span></span>|<span data-ttu-id="e1174-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e1174-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1174-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e1174-127">Request body</span></span>
<span data-ttu-id="e1174-128">No corpo da solicitação, forneça uma representação JSON do objeto iosLobApp.</span><span class="sxs-lookup"><span data-stu-id="e1174-128">In the request body, supply a JSON representation for the iosLobApp object.</span></span>

<span data-ttu-id="e1174-129">A tabela a seguir mostra as propriedades obrigatórias ao criar iosLobApp.</span><span class="sxs-lookup"><span data-stu-id="e1174-129">The following table shows the properties that are required when you create the iosLobApp.</span></span>

|<span data-ttu-id="e1174-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e1174-130">Property</span></span>|<span data-ttu-id="e1174-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e1174-131">Type</span></span>|<span data-ttu-id="e1174-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1174-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1174-133">id</span><span class="sxs-lookup"><span data-stu-id="e1174-133">id</span></span>|<span data-ttu-id="e1174-134">String</span><span class="sxs-lookup"><span data-stu-id="e1174-134">String</span></span>|<span data-ttu-id="e1174-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e1174-135">Key of the entity.</span></span> <span data-ttu-id="e1174-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e1174-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e1174-137">displayName</span><span class="sxs-lookup"><span data-stu-id="e1174-137">displayName</span></span>|<span data-ttu-id="e1174-138">String</span><span class="sxs-lookup"><span data-stu-id="e1174-138">String</span></span>|<span data-ttu-id="e1174-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="e1174-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="e1174-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e1174-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e1174-141">description</span><span class="sxs-lookup"><span data-stu-id="e1174-141">description</span></span>|<span data-ttu-id="e1174-142">String</span><span class="sxs-lookup"><span data-stu-id="e1174-142">String</span></span>|<span data-ttu-id="e1174-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e1174-143">The description of the app.</span></span> <span data-ttu-id="e1174-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e1174-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e1174-145">publicador</span><span class="sxs-lookup"><span data-stu-id="e1174-145">publisher</span></span>|<span data-ttu-id="e1174-146">String</span><span class="sxs-lookup"><span data-stu-id="e1174-146">String</span></span>|<span data-ttu-id="e1174-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e1174-147">The publisher of the app.</span></span> <span data-ttu-id="e1174-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e1174-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e1174-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e1174-149">largeIcon</span></span>|[<span data-ttu-id="e1174-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e1174-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e1174-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="e1174-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="e1174-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e1174-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e1174-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e1174-153">createdDateTime</span></span>|<span data-ttu-id="e1174-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1174-154">DateTimeOffset</span></span>|<span data-ttu-id="e1174-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e1174-155">The date and time the app was created.</span></span> <span data-ttu-id="e1174-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e1174-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e1174-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e1174-157">lastModifiedDateTime</span></span>|<span data-ttu-id="e1174-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1174-158">DateTimeOffset</span></span>|<span data-ttu-id="e1174-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="e1174-159">The date and time the app was last modified.</span></span> <span data-ttu-id="e1174-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e1174-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e1174-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e1174-161">isFeatured</span></span>|<span data-ttu-id="e1174-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1174-162">Boolean</span></span>|<span data-ttu-id="e1174-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e1174-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e1174-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e1174-164">privacyInformationUrl</span></span>|<span data-ttu-id="e1174-165">String</span><span class="sxs-lookup"><span data-stu-id="e1174-165">String</span></span>|<span data-ttu-id="e1174-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="e1174-166">The privacy statement Url.</span></span> <span data-ttu-id="e1174-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e1174-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e1174-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e1174-168">informationUrl</span></span>|<span data-ttu-id="e1174-169">String</span><span class="sxs-lookup"><span data-stu-id="e1174-169">String</span></span>|<span data-ttu-id="e1174-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="e1174-170">The more information Url.</span></span> <span data-ttu-id="e1174-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e1174-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e1174-172">owner</span><span class="sxs-lookup"><span data-stu-id="e1174-172">owner</span></span>|<span data-ttu-id="e1174-173">String</span><span class="sxs-lookup"><span data-stu-id="e1174-173">String</span></span>|<span data-ttu-id="e1174-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="e1174-174">The owner of the app.</span></span> <span data-ttu-id="e1174-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e1174-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e1174-176">developer</span><span class="sxs-lookup"><span data-stu-id="e1174-176">developer</span></span>|<span data-ttu-id="e1174-177">String</span><span class="sxs-lookup"><span data-stu-id="e1174-177">String</span></span>|<span data-ttu-id="e1174-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e1174-178">The developer of the app.</span></span> <span data-ttu-id="e1174-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e1174-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e1174-180">notes</span><span class="sxs-lookup"><span data-stu-id="e1174-180">notes</span></span>|<span data-ttu-id="e1174-181">String</span><span class="sxs-lookup"><span data-stu-id="e1174-181">String</span></span>|<span data-ttu-id="e1174-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e1174-182">Notes for the app.</span></span> <span data-ttu-id="e1174-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e1174-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e1174-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="e1174-184">uploadState</span></span>|<span data-ttu-id="e1174-185">Int32</span><span class="sxs-lookup"><span data-stu-id="e1174-185">Int32</span></span>|<span data-ttu-id="e1174-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="e1174-186">The upload state.</span></span> <span data-ttu-id="e1174-187">Os valores possíveis são: 0 - `Not Ready` , 1 - `Ready` , 2 - `Processing` .</span><span class="sxs-lookup"><span data-stu-id="e1174-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="e1174-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e1174-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e1174-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="e1174-189">publishingState</span></span>|[<span data-ttu-id="e1174-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="e1174-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="e1174-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e1174-191">The publishing state for the app.</span></span> <span data-ttu-id="e1174-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="e1174-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="e1174-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e1174-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="e1174-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="e1174-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="e1174-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="e1174-195">isAssigned</span></span>|<span data-ttu-id="e1174-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1174-196">Boolean</span></span>|<span data-ttu-id="e1174-197">O valor que indica se o aplicativo está atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="e1174-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="e1174-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e1174-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e1174-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e1174-199">roleScopeTagIds</span></span>|<span data-ttu-id="e1174-200">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e1174-200">String collection</span></span>|<span data-ttu-id="e1174-201">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="e1174-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="e1174-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e1174-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e1174-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="e1174-203">dependentAppCount</span></span>|<span data-ttu-id="e1174-204">Int32</span><span class="sxs-lookup"><span data-stu-id="e1174-204">Int32</span></span>|<span data-ttu-id="e1174-205">O número total de dependências que o aplicativo filho tem.</span><span class="sxs-lookup"><span data-stu-id="e1174-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="e1174-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e1174-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e1174-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="e1174-207">supersedingAppCount</span></span>|<span data-ttu-id="e1174-208">Int32</span><span class="sxs-lookup"><span data-stu-id="e1174-208">Int32</span></span>|<span data-ttu-id="e1174-209">O número total de aplicativos que este aplicativo é direta ou indiretamente é supersedido.</span><span class="sxs-lookup"><span data-stu-id="e1174-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="e1174-210">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e1174-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e1174-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="e1174-211">supersededAppCount</span></span>|<span data-ttu-id="e1174-212">Int32</span><span class="sxs-lookup"><span data-stu-id="e1174-212">Int32</span></span>|<span data-ttu-id="e1174-213">O número total de aplicativos pelos quais esse aplicativo é direta ou indiretamente sobressu valorado.</span><span class="sxs-lookup"><span data-stu-id="e1174-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="e1174-214">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e1174-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e1174-215">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="e1174-215">committedContentVersion</span></span>|<span data-ttu-id="e1174-216">String</span><span class="sxs-lookup"><span data-stu-id="e1174-216">String</span></span>|<span data-ttu-id="e1174-217">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="e1174-217">The internal committed content version.</span></span> <span data-ttu-id="e1174-218">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="e1174-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e1174-219">fileName</span><span class="sxs-lookup"><span data-stu-id="e1174-219">fileName</span></span>|<span data-ttu-id="e1174-220">String</span><span class="sxs-lookup"><span data-stu-id="e1174-220">String</span></span>|<span data-ttu-id="e1174-221">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="e1174-221">The name of the main Lob application file.</span></span> <span data-ttu-id="e1174-222">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="e1174-222">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e1174-223">size</span><span class="sxs-lookup"><span data-stu-id="e1174-223">size</span></span>|<span data-ttu-id="e1174-224">Int64</span><span class="sxs-lookup"><span data-stu-id="e1174-224">Int64</span></span>|<span data-ttu-id="e1174-225">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="e1174-225">The total size, including all uploaded files.</span></span> <span data-ttu-id="e1174-226">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="e1174-226">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e1174-227">bundleId</span><span class="sxs-lookup"><span data-stu-id="e1174-227">bundleId</span></span>|<span data-ttu-id="e1174-228">String</span><span class="sxs-lookup"><span data-stu-id="e1174-228">String</span></span>|<span data-ttu-id="e1174-229">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="e1174-229">The Identity Name.</span></span>|
|<span data-ttu-id="e1174-230">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="e1174-230">applicableDeviceType</span></span>|[<span data-ttu-id="e1174-231">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="e1174-231">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="e1174-232">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="e1174-232">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="e1174-233">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e1174-233">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="e1174-234">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e1174-234">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="e1174-235">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="e1174-235">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="e1174-236">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="e1174-236">expirationDateTime</span></span>|<span data-ttu-id="e1174-237">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1174-237">DateTimeOffset</span></span>|<span data-ttu-id="e1174-238">O tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="e1174-238">The expiration time.</span></span>|
|<span data-ttu-id="e1174-239">versionNumber</span><span class="sxs-lookup"><span data-stu-id="e1174-239">versionNumber</span></span>|<span data-ttu-id="e1174-240">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e1174-240">String</span></span>|<span data-ttu-id="e1174-241">O número de versão do aplicativo de Linha de Negócios (LoB) iOS.</span><span class="sxs-lookup"><span data-stu-id="e1174-241">The version number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="e1174-242">buildNumber</span><span class="sxs-lookup"><span data-stu-id="e1174-242">buildNumber</span></span>|<span data-ttu-id="e1174-243">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e1174-243">String</span></span>|<span data-ttu-id="e1174-244">O número de build do aplicativo de Linha de Negócios (LoB) iOS.</span><span class="sxs-lookup"><span data-stu-id="e1174-244">The build number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="e1174-245">identityVersion</span><span class="sxs-lookup"><span data-stu-id="e1174-245">identityVersion</span></span>|<span data-ttu-id="e1174-246">String</span><span class="sxs-lookup"><span data-stu-id="e1174-246">String</span></span>|<span data-ttu-id="e1174-247">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="e1174-247">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="e1174-248">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1174-248">Response</span></span>
<span data-ttu-id="e1174-249">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [iosLobApp](../resources/intune-apps-ioslobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e1174-249">If successful, this method returns a `201 Created` response code and a [iosLobApp](../resources/intune-apps-ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1174-250">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e1174-250">Example</span></span>

### <a name="request"></a><span data-ttu-id="e1174-251">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e1174-251">Request</span></span>
<span data-ttu-id="e1174-252">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e1174-252">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1488

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
    "v13_0": true,
    "v14_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="e1174-253">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1174-253">Response</span></span>
<span data-ttu-id="e1174-p124">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e1174-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1660

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
    "v13_0": true,
    "v14_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```




