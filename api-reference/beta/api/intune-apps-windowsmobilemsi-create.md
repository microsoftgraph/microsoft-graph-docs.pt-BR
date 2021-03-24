---
title: Criar windowsMobileMSI
description: Cria um novo objeto windowsMobileMSI.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 28340a1f687975ded95b5229c3683713a809cb1c
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51138959"
---
# <a name="create-windowsmobilemsi"></a><span data-ttu-id="04b4b-103">Criar windowsMobileMSI</span><span class="sxs-lookup"><span data-stu-id="04b4b-103">Create windowsMobileMSI</span></span>

<span data-ttu-id="04b4b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04b4b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="04b4b-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="04b4b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="04b4b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="04b4b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04b4b-107">Cria um novo objeto [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="04b4b-107">Create a new [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="04b4b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="04b4b-108">Prerequisites</span></span>
<span data-ttu-id="04b4b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04b4b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04b4b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="04b4b-111">Permission type</span></span>|<span data-ttu-id="04b4b-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="04b4b-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04b4b-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="04b4b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="04b4b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04b4b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="04b4b-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="04b4b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04b4b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="04b4b-116">Not supported.</span></span>|
|<span data-ttu-id="04b4b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="04b4b-117">Application</span></span>|<span data-ttu-id="04b4b-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04b4b-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="04b4b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="04b4b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="04b4b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="04b4b-120">Request headers</span></span>
|<span data-ttu-id="04b4b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="04b4b-121">Header</span></span>|<span data-ttu-id="04b4b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="04b4b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04b4b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="04b4b-123">Authorization</span></span>|<span data-ttu-id="04b4b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="04b4b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04b4b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="04b4b-125">Accept</span></span>|<span data-ttu-id="04b4b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="04b4b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04b4b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="04b4b-127">Request body</span></span>
<span data-ttu-id="04b4b-128">No corpo da solicitação, forneça uma representação JSON para o objeto windowsMobileMSI.</span><span class="sxs-lookup"><span data-stu-id="04b4b-128">In the request body, supply a JSON representation for the windowsMobileMSI object.</span></span>

<span data-ttu-id="04b4b-129">A tabela a seguir mostra as propriedades obrigatórias ao criar windowsMobileMSI.</span><span class="sxs-lookup"><span data-stu-id="04b4b-129">The following table shows the properties that are required when you create the windowsMobileMSI.</span></span>

|<span data-ttu-id="04b4b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="04b4b-130">Property</span></span>|<span data-ttu-id="04b4b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="04b4b-131">Type</span></span>|<span data-ttu-id="04b4b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="04b4b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04b4b-133">id</span><span class="sxs-lookup"><span data-stu-id="04b4b-133">id</span></span>|<span data-ttu-id="04b4b-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="04b4b-134">String</span></span>|<span data-ttu-id="04b4b-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="04b4b-135">Key of the entity.</span></span> <span data-ttu-id="04b4b-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="04b4b-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="04b4b-137">displayName</span><span class="sxs-lookup"><span data-stu-id="04b4b-137">displayName</span></span>|<span data-ttu-id="04b4b-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="04b4b-138">String</span></span>|<span data-ttu-id="04b4b-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="04b4b-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="04b4b-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="04b4b-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="04b4b-141">descrição</span><span class="sxs-lookup"><span data-stu-id="04b4b-141">description</span></span>|<span data-ttu-id="04b4b-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="04b4b-142">String</span></span>|<span data-ttu-id="04b4b-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="04b4b-143">The description of the app.</span></span> <span data-ttu-id="04b4b-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="04b4b-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="04b4b-145">publicador</span><span class="sxs-lookup"><span data-stu-id="04b4b-145">publisher</span></span>|<span data-ttu-id="04b4b-146">String</span><span class="sxs-lookup"><span data-stu-id="04b4b-146">String</span></span>|<span data-ttu-id="04b4b-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="04b4b-147">The publisher of the app.</span></span> <span data-ttu-id="04b4b-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="04b4b-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="04b4b-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="04b4b-149">largeIcon</span></span>|[<span data-ttu-id="04b4b-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="04b4b-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="04b4b-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="04b4b-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="04b4b-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="04b4b-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="04b4b-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="04b4b-153">createdDateTime</span></span>|<span data-ttu-id="04b4b-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="04b4b-154">DateTimeOffset</span></span>|<span data-ttu-id="04b4b-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="04b4b-155">The date and time the app was created.</span></span> <span data-ttu-id="04b4b-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="04b4b-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="04b4b-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="04b4b-157">lastModifiedDateTime</span></span>|<span data-ttu-id="04b4b-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="04b4b-158">DateTimeOffset</span></span>|<span data-ttu-id="04b4b-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="04b4b-159">The date and time the app was last modified.</span></span> <span data-ttu-id="04b4b-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="04b4b-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="04b4b-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="04b4b-161">isFeatured</span></span>|<span data-ttu-id="04b4b-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="04b4b-162">Boolean</span></span>|<span data-ttu-id="04b4b-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="04b4b-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="04b4b-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="04b4b-164">privacyInformationUrl</span></span>|<span data-ttu-id="04b4b-165">String</span><span class="sxs-lookup"><span data-stu-id="04b4b-165">String</span></span>|<span data-ttu-id="04b4b-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="04b4b-166">The privacy statement Url.</span></span> <span data-ttu-id="04b4b-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="04b4b-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="04b4b-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="04b4b-168">informationUrl</span></span>|<span data-ttu-id="04b4b-169">String</span><span class="sxs-lookup"><span data-stu-id="04b4b-169">String</span></span>|<span data-ttu-id="04b4b-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="04b4b-170">The more information Url.</span></span> <span data-ttu-id="04b4b-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="04b4b-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="04b4b-172">owner</span><span class="sxs-lookup"><span data-stu-id="04b4b-172">owner</span></span>|<span data-ttu-id="04b4b-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="04b4b-173">String</span></span>|<span data-ttu-id="04b4b-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="04b4b-174">The owner of the app.</span></span> <span data-ttu-id="04b4b-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="04b4b-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="04b4b-176">developer</span><span class="sxs-lookup"><span data-stu-id="04b4b-176">developer</span></span>|<span data-ttu-id="04b4b-177">String</span><span class="sxs-lookup"><span data-stu-id="04b4b-177">String</span></span>|<span data-ttu-id="04b4b-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="04b4b-178">The developer of the app.</span></span> <span data-ttu-id="04b4b-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="04b4b-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="04b4b-180">notes</span><span class="sxs-lookup"><span data-stu-id="04b4b-180">notes</span></span>|<span data-ttu-id="04b4b-181">String</span><span class="sxs-lookup"><span data-stu-id="04b4b-181">String</span></span>|<span data-ttu-id="04b4b-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="04b4b-182">Notes for the app.</span></span> <span data-ttu-id="04b4b-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="04b4b-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="04b4b-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="04b4b-184">uploadState</span></span>|<span data-ttu-id="04b4b-185">Int32</span><span class="sxs-lookup"><span data-stu-id="04b4b-185">Int32</span></span>|<span data-ttu-id="04b4b-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="04b4b-186">The upload state.</span></span> <span data-ttu-id="04b4b-187">Os valores possíveis são: 0 - `Not Ready` , 1 - `Ready` , 2 - `Processing` .</span><span class="sxs-lookup"><span data-stu-id="04b4b-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="04b4b-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="04b4b-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="04b4b-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="04b4b-189">publishingState</span></span>|[<span data-ttu-id="04b4b-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="04b4b-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="04b4b-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="04b4b-191">The publishing state for the app.</span></span> <span data-ttu-id="04b4b-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="04b4b-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="04b4b-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="04b4b-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="04b4b-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="04b4b-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="04b4b-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="04b4b-195">isAssigned</span></span>|<span data-ttu-id="04b4b-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="04b4b-196">Boolean</span></span>|<span data-ttu-id="04b4b-197">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="04b4b-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="04b4b-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="04b4b-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="04b4b-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="04b4b-199">roleScopeTagIds</span></span>|<span data-ttu-id="04b4b-200">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="04b4b-200">String collection</span></span>|<span data-ttu-id="04b4b-201">Lista de ids de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="04b4b-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="04b4b-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="04b4b-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="04b4b-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="04b4b-203">dependentAppCount</span></span>|<span data-ttu-id="04b4b-204">Int32</span><span class="sxs-lookup"><span data-stu-id="04b4b-204">Int32</span></span>|<span data-ttu-id="04b4b-205">O número total de dependências que o aplicativo filho tem.</span><span class="sxs-lookup"><span data-stu-id="04b4b-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="04b4b-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="04b4b-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="04b4b-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="04b4b-207">supersedingAppCount</span></span>|<span data-ttu-id="04b4b-208">Int32</span><span class="sxs-lookup"><span data-stu-id="04b4b-208">Int32</span></span>|<span data-ttu-id="04b4b-209">O número total de aplicativos que esse aplicativo sobressede direta ou indiretamente.</span><span class="sxs-lookup"><span data-stu-id="04b4b-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="04b4b-210">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="04b4b-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="04b4b-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="04b4b-211">supersededAppCount</span></span>|<span data-ttu-id="04b4b-212">Int32</span><span class="sxs-lookup"><span data-stu-id="04b4b-212">Int32</span></span>|<span data-ttu-id="04b4b-213">O número total de aplicativos pelos quais esse aplicativo é, direta ou indiretamente, é suplido.</span><span class="sxs-lookup"><span data-stu-id="04b4b-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="04b4b-214">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="04b4b-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="04b4b-215">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="04b4b-215">committedContentVersion</span></span>|<span data-ttu-id="04b4b-216">String</span><span class="sxs-lookup"><span data-stu-id="04b4b-216">String</span></span>|<span data-ttu-id="04b4b-217">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="04b4b-217">The internal committed content version.</span></span> <span data-ttu-id="04b4b-218">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="04b4b-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="04b4b-219">fileName</span><span class="sxs-lookup"><span data-stu-id="04b4b-219">fileName</span></span>|<span data-ttu-id="04b4b-220">String</span><span class="sxs-lookup"><span data-stu-id="04b4b-220">String</span></span>|<span data-ttu-id="04b4b-221">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="04b4b-221">The name of the main Lob application file.</span></span> <span data-ttu-id="04b4b-222">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="04b4b-222">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="04b4b-223">size</span><span class="sxs-lookup"><span data-stu-id="04b4b-223">size</span></span>|<span data-ttu-id="04b4b-224">Int64</span><span class="sxs-lookup"><span data-stu-id="04b4b-224">Int64</span></span>|<span data-ttu-id="04b4b-225">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="04b4b-225">The total size, including all uploaded files.</span></span> <span data-ttu-id="04b4b-226">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="04b4b-226">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="04b4b-227">commandLine</span><span class="sxs-lookup"><span data-stu-id="04b4b-227">commandLine</span></span>|<span data-ttu-id="04b4b-228">String</span><span class="sxs-lookup"><span data-stu-id="04b4b-228">String</span></span>|<span data-ttu-id="04b4b-229">A linha de comando.</span><span class="sxs-lookup"><span data-stu-id="04b4b-229">The command line.</span></span>|
|<span data-ttu-id="04b4b-230">productCode</span><span class="sxs-lookup"><span data-stu-id="04b4b-230">productCode</span></span>|<span data-ttu-id="04b4b-231">String</span><span class="sxs-lookup"><span data-stu-id="04b4b-231">String</span></span>|<span data-ttu-id="04b4b-232">O código do produto.</span><span class="sxs-lookup"><span data-stu-id="04b4b-232">The product code.</span></span>|
|<span data-ttu-id="04b4b-233">productVersion</span><span class="sxs-lookup"><span data-stu-id="04b4b-233">productVersion</span></span>|<span data-ttu-id="04b4b-234">String</span><span class="sxs-lookup"><span data-stu-id="04b4b-234">String</span></span>|<span data-ttu-id="04b4b-235">A versão de produto do aplicativo de linha de negócios (LoB) Windows Mobile MSI.</span><span class="sxs-lookup"><span data-stu-id="04b4b-235">The product version of Windows Mobile MSI Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="04b4b-236">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="04b4b-236">ignoreVersionDetection</span></span>|<span data-ttu-id="04b4b-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="04b4b-237">Boolean</span></span>|<span data-ttu-id="04b4b-238">Um booliano para controlar se a versão do aplicativo será usada para detectar o aplicativo depois que ele for instalado em um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="04b4b-238">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="04b4b-239">Defina como true para o aplicativos de linha de negócios (LoB) Windows Mobile MSI que usam um recurso de atualização automática.</span><span class="sxs-lookup"><span data-stu-id="04b4b-239">Set this to true for Windows Mobile MSI Line of Business (LoB) apps that use a self update feature.</span></span>|
|<span data-ttu-id="04b4b-240">identityVersion</span><span class="sxs-lookup"><span data-stu-id="04b4b-240">identityVersion</span></span>|<span data-ttu-id="04b4b-241">String</span><span class="sxs-lookup"><span data-stu-id="04b4b-241">String</span></span>|<span data-ttu-id="04b4b-242">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="04b4b-242">The identity version.</span></span>|
|<span data-ttu-id="04b4b-243">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="04b4b-243">useDeviceContext</span></span>|<span data-ttu-id="04b4b-244">Booliano</span><span class="sxs-lookup"><span data-stu-id="04b4b-244">Boolean</span></span>|<span data-ttu-id="04b4b-245">Indica se é preciso instalar um MSI de modo duplo no contexto do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="04b4b-245">Indicates whether to install a dual-mode MSI in the device context.</span></span> <span data-ttu-id="04b4b-246">Se for true, o aplicativo será instalado para todos os usuários.</span><span class="sxs-lookup"><span data-stu-id="04b4b-246">If true, app will be installed for all users.</span></span> <span data-ttu-id="04b4b-247">Se false, o aplicativo será instalado por usuário.</span><span class="sxs-lookup"><span data-stu-id="04b4b-247">If false, app will be installed per-user.</span></span> <span data-ttu-id="04b4b-248">Se nulo, o serviço usará o contexto de instalação padrão do pacote MSI.</span><span class="sxs-lookup"><span data-stu-id="04b4b-248">If null, service will use the MSI package's default install context.</span></span> <span data-ttu-id="04b4b-249">No caso de MSI de modo duplo, esse padrão será por usuário.</span><span class="sxs-lookup"><span data-stu-id="04b4b-249">In case of dual-mode MSI, this default will be per-user.</span></span>  <span data-ttu-id="04b4b-250">Não é possível definir aplicativos de modo não dual.</span><span class="sxs-lookup"><span data-stu-id="04b4b-250">Cannot be set for non-dual-mode apps.</span></span>  <span data-ttu-id="04b4b-251">Não é possível mudar após a criação inicial do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="04b4b-251">Cannot be changed after initial creation of the application.</span></span>|



## <a name="response"></a><span data-ttu-id="04b4b-252">Resposta</span><span class="sxs-lookup"><span data-stu-id="04b4b-252">Response</span></span>
<span data-ttu-id="04b4b-253">Se tiver êxito, este método retornará o código de resposta `201 Created` e o objeto [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="04b4b-253">If successful, this method returns a `201 Created` response code and a [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04b4b-254">Exemplo</span><span class="sxs-lookup"><span data-stu-id="04b4b-254">Example</span></span>

### <a name="request"></a><span data-ttu-id="04b4b-255">Solicitação</span><span class="sxs-lookup"><span data-stu-id="04b4b-255">Request</span></span>
<span data-ttu-id="04b4b-256">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="04b4b-256">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1123

{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
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
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true,
  "identityVersion": "Identity Version value",
  "useDeviceContext": true
}
```

### <a name="response"></a><span data-ttu-id="04b4b-257">Resposta</span><span class="sxs-lookup"><span data-stu-id="04b4b-257">Response</span></span>
<span data-ttu-id="04b4b-p126">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="04b4b-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1295

{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
  "id": "aa453e5d-3e5d-aa45-5d3e-45aa5d3e45aa",
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
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true,
  "identityVersion": "Identity Version value",
  "useDeviceContext": true
}
```




