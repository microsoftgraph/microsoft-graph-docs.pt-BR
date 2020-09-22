---
title: Criar windowsPhone81AppX
description: Criar um novo objeto windowsPhone81AppX.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 417e8b0c23c25f19e267ddf5ed55a2c1ed81898f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47976428"
---
# <a name="create-windowsphone81appx"></a><span data-ttu-id="e47e4-103">Criar windowsPhone81AppX</span><span class="sxs-lookup"><span data-stu-id="e47e4-103">Create windowsPhone81AppX</span></span>

<span data-ttu-id="e47e4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e47e4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e47e4-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e47e4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e47e4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e47e4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e47e4-107">Criar um novo objeto [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) .</span><span class="sxs-lookup"><span data-stu-id="e47e4-107">Create a new [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e47e4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e47e4-108">Prerequisites</span></span>
<span data-ttu-id="e47e4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e47e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e47e4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e47e4-111">Permission type</span></span>|<span data-ttu-id="e47e4-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e47e4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e47e4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e47e4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e47e4-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e47e4-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e47e4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e47e4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e47e4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e47e4-116">Not supported.</span></span>|
|<span data-ttu-id="e47e4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e47e4-117">Application</span></span>|<span data-ttu-id="e47e4-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e47e4-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e47e4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e47e4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="e47e4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e47e4-120">Request headers</span></span>
|<span data-ttu-id="e47e4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e47e4-121">Header</span></span>|<span data-ttu-id="e47e4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e47e4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e47e4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e47e4-123">Authorization</span></span>|<span data-ttu-id="e47e4-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e47e4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e47e4-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e47e4-125">Accept</span></span>|<span data-ttu-id="e47e4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e47e4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e47e4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e47e4-127">Request body</span></span>
<span data-ttu-id="e47e4-128">No corpo da solicitação, forneça uma representação JSON do objeto windowsPhone81AppX.</span><span class="sxs-lookup"><span data-stu-id="e47e4-128">In the request body, supply a JSON representation for the windowsPhone81AppX object.</span></span>

<span data-ttu-id="e47e4-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsPhone81AppX.</span><span class="sxs-lookup"><span data-stu-id="e47e4-129">The following table shows the properties that are required when you create the windowsPhone81AppX.</span></span>

|<span data-ttu-id="e47e4-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e47e4-130">Property</span></span>|<span data-ttu-id="e47e4-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e47e4-131">Type</span></span>|<span data-ttu-id="e47e4-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e47e4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e47e4-133">id</span><span class="sxs-lookup"><span data-stu-id="e47e4-133">id</span></span>|<span data-ttu-id="e47e4-134">String</span><span class="sxs-lookup"><span data-stu-id="e47e4-134">String</span></span>|<span data-ttu-id="e47e4-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e47e4-135">Key of the entity.</span></span> <span data-ttu-id="e47e4-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e47e4-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e47e4-137">displayName</span><span class="sxs-lookup"><span data-stu-id="e47e4-137">displayName</span></span>|<span data-ttu-id="e47e4-138">String</span><span class="sxs-lookup"><span data-stu-id="e47e4-138">String</span></span>|<span data-ttu-id="e47e4-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="e47e4-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="e47e4-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e47e4-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e47e4-141">description</span><span class="sxs-lookup"><span data-stu-id="e47e4-141">description</span></span>|<span data-ttu-id="e47e4-142">String</span><span class="sxs-lookup"><span data-stu-id="e47e4-142">String</span></span>|<span data-ttu-id="e47e4-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e47e4-143">The description of the app.</span></span> <span data-ttu-id="e47e4-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e47e4-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e47e4-145">publicador</span><span class="sxs-lookup"><span data-stu-id="e47e4-145">publisher</span></span>|<span data-ttu-id="e47e4-146">String</span><span class="sxs-lookup"><span data-stu-id="e47e4-146">String</span></span>|<span data-ttu-id="e47e4-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e47e4-147">The publisher of the app.</span></span> <span data-ttu-id="e47e4-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e47e4-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e47e4-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e47e4-149">largeIcon</span></span>|[<span data-ttu-id="e47e4-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e47e4-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e47e4-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="e47e4-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="e47e4-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e47e4-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e47e4-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e47e4-153">createdDateTime</span></span>|<span data-ttu-id="e47e4-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e47e4-154">DateTimeOffset</span></span>|<span data-ttu-id="e47e4-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e47e4-155">The date and time the app was created.</span></span> <span data-ttu-id="e47e4-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e47e4-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e47e4-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e47e4-157">lastModifiedDateTime</span></span>|<span data-ttu-id="e47e4-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e47e4-158">DateTimeOffset</span></span>|<span data-ttu-id="e47e4-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="e47e4-159">The date and time the app was last modified.</span></span> <span data-ttu-id="e47e4-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e47e4-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e47e4-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e47e4-161">isFeatured</span></span>|<span data-ttu-id="e47e4-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="e47e4-162">Boolean</span></span>|<span data-ttu-id="e47e4-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e47e4-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e47e4-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e47e4-164">privacyInformationUrl</span></span>|<span data-ttu-id="e47e4-165">String</span><span class="sxs-lookup"><span data-stu-id="e47e4-165">String</span></span>|<span data-ttu-id="e47e4-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="e47e4-166">The privacy statement Url.</span></span> <span data-ttu-id="e47e4-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e47e4-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e47e4-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e47e4-168">informationUrl</span></span>|<span data-ttu-id="e47e4-169">String</span><span class="sxs-lookup"><span data-stu-id="e47e4-169">String</span></span>|<span data-ttu-id="e47e4-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="e47e4-170">The more information Url.</span></span> <span data-ttu-id="e47e4-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e47e4-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e47e4-172">proprietário</span><span class="sxs-lookup"><span data-stu-id="e47e4-172">owner</span></span>|<span data-ttu-id="e47e4-173">String</span><span class="sxs-lookup"><span data-stu-id="e47e4-173">String</span></span>|<span data-ttu-id="e47e4-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="e47e4-174">The owner of the app.</span></span> <span data-ttu-id="e47e4-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e47e4-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e47e4-176">developer</span><span class="sxs-lookup"><span data-stu-id="e47e4-176">developer</span></span>|<span data-ttu-id="e47e4-177">String</span><span class="sxs-lookup"><span data-stu-id="e47e4-177">String</span></span>|<span data-ttu-id="e47e4-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e47e4-178">The developer of the app.</span></span> <span data-ttu-id="e47e4-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e47e4-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e47e4-180">notes</span><span class="sxs-lookup"><span data-stu-id="e47e4-180">notes</span></span>|<span data-ttu-id="e47e4-181">String</span><span class="sxs-lookup"><span data-stu-id="e47e4-181">String</span></span>|<span data-ttu-id="e47e4-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e47e4-182">Notes for the app.</span></span> <span data-ttu-id="e47e4-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e47e4-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e47e4-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="e47e4-184">uploadState</span></span>|<span data-ttu-id="e47e4-185">Int32</span><span class="sxs-lookup"><span data-stu-id="e47e4-185">Int32</span></span>|<span data-ttu-id="e47e4-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="e47e4-186">The upload state.</span></span> <span data-ttu-id="e47e4-187">Os valores possíveis são: 0- `Not Ready` , 1- `Ready` , 2- `Processing` .</span><span class="sxs-lookup"><span data-stu-id="e47e4-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="e47e4-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e47e4-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e47e4-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="e47e4-189">publishingState</span></span>|[<span data-ttu-id="e47e4-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="e47e4-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="e47e4-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e47e4-191">The publishing state for the app.</span></span> <span data-ttu-id="e47e4-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="e47e4-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="e47e4-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e47e4-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="e47e4-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="e47e4-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="e47e4-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="e47e4-195">isAssigned</span></span>|<span data-ttu-id="e47e4-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="e47e4-196">Boolean</span></span>|<span data-ttu-id="e47e4-197">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="e47e4-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="e47e4-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e47e4-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e47e4-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e47e4-199">roleScopeTagIds</span></span>|<span data-ttu-id="e47e4-200">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e47e4-200">String collection</span></span>|<span data-ttu-id="e47e4-201">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="e47e4-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="e47e4-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e47e4-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e47e4-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="e47e4-203">dependentAppCount</span></span>|<span data-ttu-id="e47e4-204">Int32</span><span class="sxs-lookup"><span data-stu-id="e47e4-204">Int32</span></span>|<span data-ttu-id="e47e4-205">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="e47e4-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="e47e4-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e47e4-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e47e4-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="e47e4-207">supersedingAppCount</span></span>|<span data-ttu-id="e47e4-208">Int32</span><span class="sxs-lookup"><span data-stu-id="e47e4-208">Int32</span></span>|<span data-ttu-id="e47e4-209">O número total de aplicativos que este aplicativo substitui direta ou indiretamente.</span><span class="sxs-lookup"><span data-stu-id="e47e4-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="e47e4-210">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e47e4-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e47e4-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="e47e4-211">supersededAppCount</span></span>|<span data-ttu-id="e47e4-212">Int32</span><span class="sxs-lookup"><span data-stu-id="e47e4-212">Int32</span></span>|<span data-ttu-id="e47e4-213">O número total de aplicativos que este aplicativo está substituindo direta ou indiretamente por.</span><span class="sxs-lookup"><span data-stu-id="e47e4-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="e47e4-214">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e47e4-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e47e4-215">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="e47e4-215">committedContentVersion</span></span>|<span data-ttu-id="e47e4-216">String</span><span class="sxs-lookup"><span data-stu-id="e47e4-216">String</span></span>|<span data-ttu-id="e47e4-217">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="e47e4-217">The internal committed content version.</span></span> <span data-ttu-id="e47e4-218">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="e47e4-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e47e4-219">fileName</span><span class="sxs-lookup"><span data-stu-id="e47e4-219">fileName</span></span>|<span data-ttu-id="e47e4-220">String</span><span class="sxs-lookup"><span data-stu-id="e47e4-220">String</span></span>|<span data-ttu-id="e47e4-221">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="e47e4-221">The name of the main Lob application file.</span></span> <span data-ttu-id="e47e4-222">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="e47e4-222">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e47e4-223">size</span><span class="sxs-lookup"><span data-stu-id="e47e4-223">size</span></span>|<span data-ttu-id="e47e4-224">Int64</span><span class="sxs-lookup"><span data-stu-id="e47e4-224">Int64</span></span>|<span data-ttu-id="e47e4-225">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="e47e4-225">The total size, including all uploaded files.</span></span> <span data-ttu-id="e47e4-226">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="e47e4-226">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e47e4-227">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="e47e4-227">applicableArchitectures</span></span>|[<span data-ttu-id="e47e4-228">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="e47e4-228">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="e47e4-229">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="e47e4-229">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="e47e4-230">Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="e47e4-230">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="e47e4-231">identityName</span><span class="sxs-lookup"><span data-stu-id="e47e4-231">identityName</span></span>|<span data-ttu-id="e47e4-232">String</span><span class="sxs-lookup"><span data-stu-id="e47e4-232">String</span></span>|<span data-ttu-id="e47e4-233">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="e47e4-233">The Identity Name.</span></span>|
|<span data-ttu-id="e47e4-234">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="e47e4-234">identityPublisherHash</span></span>|<span data-ttu-id="e47e4-235">String</span><span class="sxs-lookup"><span data-stu-id="e47e4-235">String</span></span>|<span data-ttu-id="e47e4-236">O Hash do Publicador de Identidade.</span><span class="sxs-lookup"><span data-stu-id="e47e4-236">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="e47e4-237">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="e47e4-237">identityResourceIdentifier</span></span>|<span data-ttu-id="e47e4-238">String</span><span class="sxs-lookup"><span data-stu-id="e47e4-238">String</span></span>|<span data-ttu-id="e47e4-239">O Identificador de Recurso da Identidade.</span><span class="sxs-lookup"><span data-stu-id="e47e4-239">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="e47e4-240">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e47e4-240">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="e47e4-241">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e47e4-241">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="e47e4-242">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="e47e4-242">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="e47e4-243">phoneProductIdentifier</span><span class="sxs-lookup"><span data-stu-id="e47e4-243">phoneProductIdentifier</span></span>|<span data-ttu-id="e47e4-244">String</span><span class="sxs-lookup"><span data-stu-id="e47e4-244">String</span></span>|<span data-ttu-id="e47e4-245">O identificador do produto de telefone.</span><span class="sxs-lookup"><span data-stu-id="e47e4-245">The Phone Product Identifier.</span></span>|
|<span data-ttu-id="e47e4-246">phonePublisherId</span><span class="sxs-lookup"><span data-stu-id="e47e4-246">phonePublisherId</span></span>|<span data-ttu-id="e47e4-247">String</span><span class="sxs-lookup"><span data-stu-id="e47e4-247">String</span></span>|<span data-ttu-id="e47e4-248">A ID do editor do telefone.</span><span class="sxs-lookup"><span data-stu-id="e47e4-248">The Phone Publisher Id.</span></span>|
|<span data-ttu-id="e47e4-249">identityVersion</span><span class="sxs-lookup"><span data-stu-id="e47e4-249">identityVersion</span></span>|<span data-ttu-id="e47e4-250">String</span><span class="sxs-lookup"><span data-stu-id="e47e4-250">String</span></span>|<span data-ttu-id="e47e4-251">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="e47e4-251">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="e47e4-252">Resposta</span><span class="sxs-lookup"><span data-stu-id="e47e4-252">Response</span></span>
<span data-ttu-id="e47e4-253">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e47e4-253">If successful, this method returns a `201 Created` response code and a [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e47e4-254">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e47e4-254">Example</span></span>

### <a name="request"></a><span data-ttu-id="e47e4-255">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e47e4-255">Request</span></span>
<span data-ttu-id="e47e4-256">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e47e4-256">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1570

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppX",
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
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="e47e4-257">Resposta</span><span class="sxs-lookup"><span data-stu-id="e47e4-257">Response</span></span>
<span data-ttu-id="e47e4-p125">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e47e4-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1742

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppX",
  "id": "4ff27f80-7f80-4ff2-807f-f24f807ff24f",
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
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value"
}
```






