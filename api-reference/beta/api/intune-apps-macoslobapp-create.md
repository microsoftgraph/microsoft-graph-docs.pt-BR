---
title: Criar macOSLobApp
description: Crie um novo objeto macOSLobApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8c8af76f072bd8b388ab1e7736b9aad0f3923912
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51862919"
---
# <a name="create-macoslobapp"></a><span data-ttu-id="f2b80-103">Criar macOSLobApp</span><span class="sxs-lookup"><span data-stu-id="f2b80-103">Create macOSLobApp</span></span>

<span data-ttu-id="f2b80-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2b80-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f2b80-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f2b80-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f2b80-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f2b80-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2b80-107">Crie um novo [objeto macOSLobApp.](../resources/intune-apps-macoslobapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2b80-107">Create a new [macOSLobApp](../resources/intune-apps-macoslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f2b80-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f2b80-108">Prerequisites</span></span>
<span data-ttu-id="f2b80-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2b80-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2b80-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f2b80-111">Permission type</span></span>|<span data-ttu-id="f2b80-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f2b80-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2b80-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f2b80-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f2b80-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2b80-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f2b80-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f2b80-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2b80-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f2b80-116">Not supported.</span></span>|
|<span data-ttu-id="f2b80-117">Application</span><span class="sxs-lookup"><span data-stu-id="f2b80-117">Application</span></span>|<span data-ttu-id="f2b80-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2b80-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2b80-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f2b80-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="f2b80-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f2b80-120">Request headers</span></span>
|<span data-ttu-id="f2b80-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f2b80-121">Header</span></span>|<span data-ttu-id="f2b80-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f2b80-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f2b80-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f2b80-123">Authorization</span></span>|<span data-ttu-id="f2b80-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f2b80-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f2b80-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f2b80-125">Accept</span></span>|<span data-ttu-id="f2b80-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f2b80-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2b80-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f2b80-127">Request body</span></span>
<span data-ttu-id="f2b80-128">No corpo da solicitação, fornece uma representação JSON para o objeto macOSLobApp.</span><span class="sxs-lookup"><span data-stu-id="f2b80-128">In the request body, supply a JSON representation for the macOSLobApp object.</span></span>

<span data-ttu-id="f2b80-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o macOSLobApp.</span><span class="sxs-lookup"><span data-stu-id="f2b80-129">The following table shows the properties that are required when you create the macOSLobApp.</span></span>

|<span data-ttu-id="f2b80-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f2b80-130">Property</span></span>|<span data-ttu-id="f2b80-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2b80-131">Type</span></span>|<span data-ttu-id="f2b80-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2b80-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2b80-133">id</span><span class="sxs-lookup"><span data-stu-id="f2b80-133">id</span></span>|<span data-ttu-id="f2b80-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2b80-134">String</span></span>|<span data-ttu-id="f2b80-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f2b80-135">Key of the entity.</span></span> <span data-ttu-id="f2b80-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2b80-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2b80-137">displayName</span><span class="sxs-lookup"><span data-stu-id="f2b80-137">displayName</span></span>|<span data-ttu-id="f2b80-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2b80-138">String</span></span>|<span data-ttu-id="f2b80-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="f2b80-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="f2b80-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2b80-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2b80-141">description</span><span class="sxs-lookup"><span data-stu-id="f2b80-141">description</span></span>|<span data-ttu-id="f2b80-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2b80-142">String</span></span>|<span data-ttu-id="f2b80-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f2b80-143">The description of the app.</span></span> <span data-ttu-id="f2b80-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2b80-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2b80-145">publicador</span><span class="sxs-lookup"><span data-stu-id="f2b80-145">publisher</span></span>|<span data-ttu-id="f2b80-146">String</span><span class="sxs-lookup"><span data-stu-id="f2b80-146">String</span></span>|<span data-ttu-id="f2b80-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f2b80-147">The publisher of the app.</span></span> <span data-ttu-id="f2b80-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2b80-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2b80-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="f2b80-149">largeIcon</span></span>|[<span data-ttu-id="f2b80-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f2b80-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f2b80-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="f2b80-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="f2b80-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2b80-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2b80-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f2b80-153">createdDateTime</span></span>|<span data-ttu-id="f2b80-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2b80-154">DateTimeOffset</span></span>|<span data-ttu-id="f2b80-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f2b80-155">The date and time the app was created.</span></span> <span data-ttu-id="f2b80-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2b80-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2b80-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f2b80-157">lastModifiedDateTime</span></span>|<span data-ttu-id="f2b80-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2b80-158">DateTimeOffset</span></span>|<span data-ttu-id="f2b80-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="f2b80-159">The date and time the app was last modified.</span></span> <span data-ttu-id="f2b80-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2b80-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2b80-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="f2b80-161">isFeatured</span></span>|<span data-ttu-id="f2b80-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="f2b80-162">Boolean</span></span>|<span data-ttu-id="f2b80-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2b80-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2b80-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f2b80-164">privacyInformationUrl</span></span>|<span data-ttu-id="f2b80-165">String</span><span class="sxs-lookup"><span data-stu-id="f2b80-165">String</span></span>|<span data-ttu-id="f2b80-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="f2b80-166">The privacy statement Url.</span></span> <span data-ttu-id="f2b80-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2b80-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2b80-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f2b80-168">informationUrl</span></span>|<span data-ttu-id="f2b80-169">String</span><span class="sxs-lookup"><span data-stu-id="f2b80-169">String</span></span>|<span data-ttu-id="f2b80-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="f2b80-170">The more information Url.</span></span> <span data-ttu-id="f2b80-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2b80-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2b80-172">owner</span><span class="sxs-lookup"><span data-stu-id="f2b80-172">owner</span></span>|<span data-ttu-id="f2b80-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2b80-173">String</span></span>|<span data-ttu-id="f2b80-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="f2b80-174">The owner of the app.</span></span> <span data-ttu-id="f2b80-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2b80-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2b80-176">developer</span><span class="sxs-lookup"><span data-stu-id="f2b80-176">developer</span></span>|<span data-ttu-id="f2b80-177">String</span><span class="sxs-lookup"><span data-stu-id="f2b80-177">String</span></span>|<span data-ttu-id="f2b80-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f2b80-178">The developer of the app.</span></span> <span data-ttu-id="f2b80-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2b80-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2b80-180">notes</span><span class="sxs-lookup"><span data-stu-id="f2b80-180">notes</span></span>|<span data-ttu-id="f2b80-181">String</span><span class="sxs-lookup"><span data-stu-id="f2b80-181">String</span></span>|<span data-ttu-id="f2b80-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f2b80-182">Notes for the app.</span></span> <span data-ttu-id="f2b80-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2b80-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2b80-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="f2b80-184">uploadState</span></span>|<span data-ttu-id="f2b80-185">Int32</span><span class="sxs-lookup"><span data-stu-id="f2b80-185">Int32</span></span>|<span data-ttu-id="f2b80-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="f2b80-186">The upload state.</span></span> <span data-ttu-id="f2b80-187">Os valores possíveis são: 0 - `Not Ready` , 1 - `Ready` , 2 - `Processing` .</span><span class="sxs-lookup"><span data-stu-id="f2b80-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="f2b80-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2b80-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2b80-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="f2b80-189">publishingState</span></span>|[<span data-ttu-id="f2b80-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="f2b80-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="f2b80-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f2b80-191">The publishing state for the app.</span></span> <span data-ttu-id="f2b80-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="f2b80-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="f2b80-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f2b80-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="f2b80-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="f2b80-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="f2b80-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="f2b80-195">isAssigned</span></span>|<span data-ttu-id="f2b80-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="f2b80-196">Boolean</span></span>|<span data-ttu-id="f2b80-197">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="f2b80-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="f2b80-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2b80-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2b80-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f2b80-199">roleScopeTagIds</span></span>|<span data-ttu-id="f2b80-200">Coleção String</span><span class="sxs-lookup"><span data-stu-id="f2b80-200">String collection</span></span>|<span data-ttu-id="f2b80-201">Lista de ids de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="f2b80-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="f2b80-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2b80-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2b80-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="f2b80-203">dependentAppCount</span></span>|<span data-ttu-id="f2b80-204">Int32</span><span class="sxs-lookup"><span data-stu-id="f2b80-204">Int32</span></span>|<span data-ttu-id="f2b80-205">O número total de dependências que o aplicativo filho tem.</span><span class="sxs-lookup"><span data-stu-id="f2b80-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="f2b80-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2b80-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2b80-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="f2b80-207">supersedingAppCount</span></span>|<span data-ttu-id="f2b80-208">Int32</span><span class="sxs-lookup"><span data-stu-id="f2b80-208">Int32</span></span>|<span data-ttu-id="f2b80-209">O número total de aplicativos que esse aplicativo sobressede direta ou indiretamente.</span><span class="sxs-lookup"><span data-stu-id="f2b80-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="f2b80-210">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2b80-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2b80-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="f2b80-211">supersededAppCount</span></span>|<span data-ttu-id="f2b80-212">Int32</span><span class="sxs-lookup"><span data-stu-id="f2b80-212">Int32</span></span>|<span data-ttu-id="f2b80-213">O número total de aplicativos pelos quais esse aplicativo é, direta ou indiretamente, é suplido.</span><span class="sxs-lookup"><span data-stu-id="f2b80-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="f2b80-214">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2b80-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2b80-215">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="f2b80-215">committedContentVersion</span></span>|<span data-ttu-id="f2b80-216">String</span><span class="sxs-lookup"><span data-stu-id="f2b80-216">String</span></span>|<span data-ttu-id="f2b80-217">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="f2b80-217">The internal committed content version.</span></span> <span data-ttu-id="f2b80-218">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2b80-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="f2b80-219">fileName</span><span class="sxs-lookup"><span data-stu-id="f2b80-219">fileName</span></span>|<span data-ttu-id="f2b80-220">String</span><span class="sxs-lookup"><span data-stu-id="f2b80-220">String</span></span>|<span data-ttu-id="f2b80-221">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="f2b80-221">The name of the main Lob application file.</span></span> <span data-ttu-id="f2b80-222">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2b80-222">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="f2b80-223">size</span><span class="sxs-lookup"><span data-stu-id="f2b80-223">size</span></span>|<span data-ttu-id="f2b80-224">Int64</span><span class="sxs-lookup"><span data-stu-id="f2b80-224">Int64</span></span>|<span data-ttu-id="f2b80-225">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="f2b80-225">The total size, including all uploaded files.</span></span> <span data-ttu-id="f2b80-226">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2b80-226">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="f2b80-227">bundleId</span><span class="sxs-lookup"><span data-stu-id="f2b80-227">bundleId</span></span>|<span data-ttu-id="f2b80-228">String</span><span class="sxs-lookup"><span data-stu-id="f2b80-228">String</span></span>|<span data-ttu-id="f2b80-229">A ID do pacote.</span><span class="sxs-lookup"><span data-stu-id="f2b80-229">The bundle id.</span></span>|
|<span data-ttu-id="f2b80-230">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f2b80-230">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="f2b80-231">macOSMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f2b80-231">macOSMinimumOperatingSystem</span></span>](../resources/intune-apps-macosminimumoperatingsystem.md)|<span data-ttu-id="f2b80-232">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="f2b80-232">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="f2b80-233">buildNumber</span><span class="sxs-lookup"><span data-stu-id="f2b80-233">buildNumber</span></span>|<span data-ttu-id="f2b80-234">String</span><span class="sxs-lookup"><span data-stu-id="f2b80-234">String</span></span>|<span data-ttu-id="f2b80-235">O número de composição do aplicativo MacOS Line of Business (LoB).</span><span class="sxs-lookup"><span data-stu-id="f2b80-235">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="f2b80-236">versionNumber</span><span class="sxs-lookup"><span data-stu-id="f2b80-236">versionNumber</span></span>|<span data-ttu-id="f2b80-237">String</span><span class="sxs-lookup"><span data-stu-id="f2b80-237">String</span></span>|<span data-ttu-id="f2b80-238">O número de versão do aplicativo MacOS Line of Business (LoB).</span><span class="sxs-lookup"><span data-stu-id="f2b80-238">The version number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="f2b80-239">childApps</span><span class="sxs-lookup"><span data-stu-id="f2b80-239">childApps</span></span>|<span data-ttu-id="f2b80-240">[Coleção macOSLobChildApp](../resources/intune-apps-macoslobchildapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2b80-240">[macOSLobChildApp](../resources/intune-apps-macoslobchildapp.md) collection</span></span>|<span data-ttu-id="f2b80-241">A lista de aplicativos neste pacote de pacotes</span><span class="sxs-lookup"><span data-stu-id="f2b80-241">The app list in this bundle package</span></span>|
|<span data-ttu-id="f2b80-242">identityVersion</span><span class="sxs-lookup"><span data-stu-id="f2b80-242">identityVersion</span></span>|<span data-ttu-id="f2b80-243">String</span><span class="sxs-lookup"><span data-stu-id="f2b80-243">String</span></span>|<span data-ttu-id="f2b80-244">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="f2b80-244">The identity version.</span></span>|
|<span data-ttu-id="f2b80-245">md5HashChunkSize</span><span class="sxs-lookup"><span data-stu-id="f2b80-245">md5HashChunkSize</span></span>|<span data-ttu-id="f2b80-246">Int32</span><span class="sxs-lookup"><span data-stu-id="f2b80-246">Int32</span></span>|<span data-ttu-id="f2b80-247">O tamanho da parte do hash MD5</span><span class="sxs-lookup"><span data-stu-id="f2b80-247">The chunk size for MD5 hash</span></span>|
|<span data-ttu-id="f2b80-248">md5Hash</span><span class="sxs-lookup"><span data-stu-id="f2b80-248">md5Hash</span></span>|<span data-ttu-id="f2b80-249">Coleção String</span><span class="sxs-lookup"><span data-stu-id="f2b80-249">String collection</span></span>|<span data-ttu-id="f2b80-250">Os códigos de hash MD5</span><span class="sxs-lookup"><span data-stu-id="f2b80-250">The MD5 hash codes</span></span>|
|<span data-ttu-id="f2b80-251">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="f2b80-251">ignoreVersionDetection</span></span>|<span data-ttu-id="f2b80-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="f2b80-252">Boolean</span></span>|<span data-ttu-id="f2b80-253">Um booliano para controlar se a versão do aplicativo será usada para detectar o aplicativo depois que ele for instalado em um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f2b80-253">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="f2b80-254">Defina isso como true para aplicativos macOS Line of Business (LoB) que usam um recurso de atualização automática.</span><span class="sxs-lookup"><span data-stu-id="f2b80-254">Set this to true for macOS Line of Business (LoB) apps that use a self update feature.</span></span>|
|<span data-ttu-id="f2b80-255">installAsManaged</span><span class="sxs-lookup"><span data-stu-id="f2b80-255">installAsManaged</span></span>|<span data-ttu-id="f2b80-256">Boolean</span><span class="sxs-lookup"><span data-stu-id="f2b80-256">Boolean</span></span>|<span data-ttu-id="f2b80-257">Um booleano para controlar se o aplicativo será instalado como gerenciado (exige macOS 11.0 e outras restrições de PKG).</span><span class="sxs-lookup"><span data-stu-id="f2b80-257">A boolean to control whether the app will be installed as managed (requires macOS 11.0 and other PKG restrictions).</span></span>|



## <a name="response"></a><span data-ttu-id="f2b80-258">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2b80-258">Response</span></span>
<span data-ttu-id="f2b80-259">Se tiver êxito, este método retornará um código `201 Created` de resposta e um objeto [macOSLobApp](../resources/intune-apps-macoslobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f2b80-259">If successful, this method returns a `201 Created` response code and a [macOSLobApp](../resources/intune-apps-macoslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2b80-260">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f2b80-260">Example</span></span>

### <a name="request"></a><span data-ttu-id="f2b80-261">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f2b80-261">Request</span></span>
<span data-ttu-id="f2b80-262">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f2b80-262">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1722

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
    "v10_15": true,
    "v11_0": true
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

### <a name="response"></a><span data-ttu-id="f2b80-263">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2b80-263">Response</span></span>
<span data-ttu-id="f2b80-p125">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f2b80-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1894

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
    "v10_15": true,
    "v11_0": true
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




