---
title: Criar androidLobApp
description: Cria um novo objeto androidLobApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 34c96864b7c874744bf9c5c1fdab8bd1c7c623e9
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51141054"
---
# <a name="create-androidlobapp"></a><span data-ttu-id="fd41c-103">Criar androidLobApp</span><span class="sxs-lookup"><span data-stu-id="fd41c-103">Create androidLobApp</span></span>

<span data-ttu-id="fd41c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fd41c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fd41c-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fd41c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fd41c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fd41c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fd41c-107">Cria um novo objeto [androidLobApp](../resources/intune-apps-androidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="fd41c-107">Create a new [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fd41c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fd41c-108">Prerequisites</span></span>
<span data-ttu-id="fd41c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd41c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd41c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fd41c-111">Permission type</span></span>|<span data-ttu-id="fd41c-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fd41c-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fd41c-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fd41c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fd41c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd41c-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fd41c-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fd41c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fd41c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fd41c-116">Not supported.</span></span>|
|<span data-ttu-id="fd41c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fd41c-117">Application</span></span>|<span data-ttu-id="fd41c-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd41c-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fd41c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fd41c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="fd41c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fd41c-120">Request headers</span></span>
|<span data-ttu-id="fd41c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fd41c-121">Header</span></span>|<span data-ttu-id="fd41c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="fd41c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fd41c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fd41c-123">Authorization</span></span>|<span data-ttu-id="fd41c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fd41c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fd41c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fd41c-125">Accept</span></span>|<span data-ttu-id="fd41c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fd41c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd41c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fd41c-127">Request body</span></span>
<span data-ttu-id="fd41c-128">No corpo da solicitação, forneça uma representação JSON do objeto androidLobApp.</span><span class="sxs-lookup"><span data-stu-id="fd41c-128">In the request body, supply a JSON representation for the androidLobApp object.</span></span>

<span data-ttu-id="fd41c-129">A tabela a seguir mostra as propriedades obrigatórias ao criar androidLobApp.</span><span class="sxs-lookup"><span data-stu-id="fd41c-129">The following table shows the properties that are required when you create the androidLobApp.</span></span>

|<span data-ttu-id="fd41c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fd41c-130">Property</span></span>|<span data-ttu-id="fd41c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="fd41c-131">Type</span></span>|<span data-ttu-id="fd41c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="fd41c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd41c-133">id</span><span class="sxs-lookup"><span data-stu-id="fd41c-133">id</span></span>|<span data-ttu-id="fd41c-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd41c-134">String</span></span>|<span data-ttu-id="fd41c-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="fd41c-135">Key of the entity.</span></span> <span data-ttu-id="fd41c-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fd41c-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fd41c-137">displayName</span><span class="sxs-lookup"><span data-stu-id="fd41c-137">displayName</span></span>|<span data-ttu-id="fd41c-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd41c-138">String</span></span>|<span data-ttu-id="fd41c-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="fd41c-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="fd41c-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fd41c-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fd41c-141">descrição</span><span class="sxs-lookup"><span data-stu-id="fd41c-141">description</span></span>|<span data-ttu-id="fd41c-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd41c-142">String</span></span>|<span data-ttu-id="fd41c-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fd41c-143">The description of the app.</span></span> <span data-ttu-id="fd41c-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fd41c-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fd41c-145">publicador</span><span class="sxs-lookup"><span data-stu-id="fd41c-145">publisher</span></span>|<span data-ttu-id="fd41c-146">String</span><span class="sxs-lookup"><span data-stu-id="fd41c-146">String</span></span>|<span data-ttu-id="fd41c-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fd41c-147">The publisher of the app.</span></span> <span data-ttu-id="fd41c-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fd41c-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fd41c-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="fd41c-149">largeIcon</span></span>|[<span data-ttu-id="fd41c-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="fd41c-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="fd41c-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="fd41c-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="fd41c-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fd41c-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fd41c-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fd41c-153">createdDateTime</span></span>|<span data-ttu-id="fd41c-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd41c-154">DateTimeOffset</span></span>|<span data-ttu-id="fd41c-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fd41c-155">The date and time the app was created.</span></span> <span data-ttu-id="fd41c-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fd41c-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fd41c-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fd41c-157">lastModifiedDateTime</span></span>|<span data-ttu-id="fd41c-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd41c-158">DateTimeOffset</span></span>|<span data-ttu-id="fd41c-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="fd41c-159">The date and time the app was last modified.</span></span> <span data-ttu-id="fd41c-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fd41c-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fd41c-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="fd41c-161">isFeatured</span></span>|<span data-ttu-id="fd41c-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="fd41c-162">Boolean</span></span>|<span data-ttu-id="fd41c-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fd41c-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fd41c-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="fd41c-164">privacyInformationUrl</span></span>|<span data-ttu-id="fd41c-165">String</span><span class="sxs-lookup"><span data-stu-id="fd41c-165">String</span></span>|<span data-ttu-id="fd41c-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="fd41c-166">The privacy statement Url.</span></span> <span data-ttu-id="fd41c-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fd41c-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fd41c-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="fd41c-168">informationUrl</span></span>|<span data-ttu-id="fd41c-169">String</span><span class="sxs-lookup"><span data-stu-id="fd41c-169">String</span></span>|<span data-ttu-id="fd41c-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="fd41c-170">The more information Url.</span></span> <span data-ttu-id="fd41c-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fd41c-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fd41c-172">owner</span><span class="sxs-lookup"><span data-stu-id="fd41c-172">owner</span></span>|<span data-ttu-id="fd41c-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd41c-173">String</span></span>|<span data-ttu-id="fd41c-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="fd41c-174">The owner of the app.</span></span> <span data-ttu-id="fd41c-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fd41c-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fd41c-176">developer</span><span class="sxs-lookup"><span data-stu-id="fd41c-176">developer</span></span>|<span data-ttu-id="fd41c-177">String</span><span class="sxs-lookup"><span data-stu-id="fd41c-177">String</span></span>|<span data-ttu-id="fd41c-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fd41c-178">The developer of the app.</span></span> <span data-ttu-id="fd41c-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fd41c-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fd41c-180">notes</span><span class="sxs-lookup"><span data-stu-id="fd41c-180">notes</span></span>|<span data-ttu-id="fd41c-181">String</span><span class="sxs-lookup"><span data-stu-id="fd41c-181">String</span></span>|<span data-ttu-id="fd41c-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fd41c-182">Notes for the app.</span></span> <span data-ttu-id="fd41c-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fd41c-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fd41c-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="fd41c-184">uploadState</span></span>|<span data-ttu-id="fd41c-185">Int32</span><span class="sxs-lookup"><span data-stu-id="fd41c-185">Int32</span></span>|<span data-ttu-id="fd41c-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="fd41c-186">The upload state.</span></span> <span data-ttu-id="fd41c-187">Os valores possíveis são: 0 - `Not Ready` , 1 - `Ready` , 2 - `Processing` .</span><span class="sxs-lookup"><span data-stu-id="fd41c-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="fd41c-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fd41c-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fd41c-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="fd41c-189">publishingState</span></span>|[<span data-ttu-id="fd41c-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="fd41c-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="fd41c-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fd41c-191">The publishing state for the app.</span></span> <span data-ttu-id="fd41c-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="fd41c-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="fd41c-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fd41c-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="fd41c-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="fd41c-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="fd41c-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="fd41c-195">isAssigned</span></span>|<span data-ttu-id="fd41c-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="fd41c-196">Boolean</span></span>|<span data-ttu-id="fd41c-197">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="fd41c-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="fd41c-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fd41c-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fd41c-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fd41c-199">roleScopeTagIds</span></span>|<span data-ttu-id="fd41c-200">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd41c-200">String collection</span></span>|<span data-ttu-id="fd41c-201">Lista de ids de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="fd41c-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="fd41c-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fd41c-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fd41c-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="fd41c-203">dependentAppCount</span></span>|<span data-ttu-id="fd41c-204">Int32</span><span class="sxs-lookup"><span data-stu-id="fd41c-204">Int32</span></span>|<span data-ttu-id="fd41c-205">O número total de dependências que o aplicativo filho tem.</span><span class="sxs-lookup"><span data-stu-id="fd41c-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="fd41c-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fd41c-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fd41c-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="fd41c-207">supersedingAppCount</span></span>|<span data-ttu-id="fd41c-208">Int32</span><span class="sxs-lookup"><span data-stu-id="fd41c-208">Int32</span></span>|<span data-ttu-id="fd41c-209">O número total de aplicativos que esse aplicativo sobressede direta ou indiretamente.</span><span class="sxs-lookup"><span data-stu-id="fd41c-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="fd41c-210">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fd41c-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fd41c-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="fd41c-211">supersededAppCount</span></span>|<span data-ttu-id="fd41c-212">Int32</span><span class="sxs-lookup"><span data-stu-id="fd41c-212">Int32</span></span>|<span data-ttu-id="fd41c-213">O número total de aplicativos pelos quais esse aplicativo é, direta ou indiretamente, é suplido.</span><span class="sxs-lookup"><span data-stu-id="fd41c-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="fd41c-214">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fd41c-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fd41c-215">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="fd41c-215">committedContentVersion</span></span>|<span data-ttu-id="fd41c-216">String</span><span class="sxs-lookup"><span data-stu-id="fd41c-216">String</span></span>|<span data-ttu-id="fd41c-217">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="fd41c-217">The internal committed content version.</span></span> <span data-ttu-id="fd41c-218">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="fd41c-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="fd41c-219">fileName</span><span class="sxs-lookup"><span data-stu-id="fd41c-219">fileName</span></span>|<span data-ttu-id="fd41c-220">String</span><span class="sxs-lookup"><span data-stu-id="fd41c-220">String</span></span>|<span data-ttu-id="fd41c-221">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="fd41c-221">The name of the main Lob application file.</span></span> <span data-ttu-id="fd41c-222">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="fd41c-222">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="fd41c-223">size</span><span class="sxs-lookup"><span data-stu-id="fd41c-223">size</span></span>|<span data-ttu-id="fd41c-224">Int64</span><span class="sxs-lookup"><span data-stu-id="fd41c-224">Int64</span></span>|<span data-ttu-id="fd41c-225">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="fd41c-225">The total size, including all uploaded files.</span></span> <span data-ttu-id="fd41c-226">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="fd41c-226">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="fd41c-227">packageId</span><span class="sxs-lookup"><span data-stu-id="fd41c-227">packageId</span></span>|<span data-ttu-id="fd41c-228">String</span><span class="sxs-lookup"><span data-stu-id="fd41c-228">String</span></span>|<span data-ttu-id="fd41c-229">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="fd41c-229">The package identifier.</span></span>|
|<span data-ttu-id="fd41c-230">identityName</span><span class="sxs-lookup"><span data-stu-id="fd41c-230">identityName</span></span>|<span data-ttu-id="fd41c-231">String</span><span class="sxs-lookup"><span data-stu-id="fd41c-231">String</span></span>|<span data-ttu-id="fd41c-232">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="fd41c-232">The Identity Name.</span></span>|
|<span data-ttu-id="fd41c-233">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="fd41c-233">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="fd41c-234">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="fd41c-234">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="fd41c-235">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="fd41c-235">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="fd41c-236">versionName</span><span class="sxs-lookup"><span data-stu-id="fd41c-236">versionName</span></span>|<span data-ttu-id="fd41c-237">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd41c-237">String</span></span>|<span data-ttu-id="fd41c-238">O nome da versão do aplicativo de Linha de Negócios (LoB) Android.</span><span class="sxs-lookup"><span data-stu-id="fd41c-238">The version name of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="fd41c-239">versionCode</span><span class="sxs-lookup"><span data-stu-id="fd41c-239">versionCode</span></span>|<span data-ttu-id="fd41c-240">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd41c-240">String</span></span>|<span data-ttu-id="fd41c-241">O código da versão do aplicativo de Linha de Negócios (LoB) Android.</span><span class="sxs-lookup"><span data-stu-id="fd41c-241">The version code of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="fd41c-242">identityVersion</span><span class="sxs-lookup"><span data-stu-id="fd41c-242">identityVersion</span></span>|<span data-ttu-id="fd41c-243">String</span><span class="sxs-lookup"><span data-stu-id="fd41c-243">String</span></span>|<span data-ttu-id="fd41c-244">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="fd41c-244">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="fd41c-245">Resposta</span><span class="sxs-lookup"><span data-stu-id="fd41c-245">Response</span></span>
<span data-ttu-id="fd41c-246">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [androidLobApp](../resources/intune-apps-androidlobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fd41c-246">If successful, this method returns a `201 Created` response code and a [androidLobApp](../resources/intune-apps-androidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd41c-247">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fd41c-247">Example</span></span>

### <a name="request"></a><span data-ttu-id="fd41c-248">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fd41c-248">Request</span></span>
<span data-ttu-id="fd41c-249">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fd41c-249">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1510

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
  "packageId": "Package Id value",
  "identityName": "Identity Name value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="fd41c-250">Resposta</span><span class="sxs-lookup"><span data-stu-id="fd41c-250">Response</span></span>
<span data-ttu-id="fd41c-p124">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fd41c-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1682

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
  "packageId": "Package Id value",
  "identityName": "Identity Name value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```




