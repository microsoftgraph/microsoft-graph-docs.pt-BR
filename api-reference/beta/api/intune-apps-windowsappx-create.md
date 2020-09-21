---
title: Criar windowsAppX
description: Criar um novo objeto windowsAppX.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9e727755634baa5b8e25fe91ece5bf833ab64793
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47976659"
---
# <a name="create-windowsappx"></a><span data-ttu-id="4f268-103">Criar windowsAppX</span><span class="sxs-lookup"><span data-stu-id="4f268-103">Create windowsAppX</span></span>

<span data-ttu-id="4f268-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f268-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4f268-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4f268-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4f268-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4f268-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f268-107">Criar um novo objeto [windowsAppX](../resources/intune-apps-windowsappx.md) .</span><span class="sxs-lookup"><span data-stu-id="4f268-107">Create a new [windowsAppX](../resources/intune-apps-windowsappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4f268-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4f268-108">Prerequisites</span></span>
<span data-ttu-id="4f268-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f268-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f268-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4f268-111">Permission type</span></span>|<span data-ttu-id="4f268-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4f268-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f268-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4f268-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4f268-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f268-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4f268-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4f268-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f268-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4f268-116">Not supported.</span></span>|
|<span data-ttu-id="4f268-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4f268-117">Application</span></span>|<span data-ttu-id="4f268-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f268-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f268-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4f268-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="4f268-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4f268-120">Request headers</span></span>
|<span data-ttu-id="4f268-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4f268-121">Header</span></span>|<span data-ttu-id="4f268-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4f268-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f268-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4f268-123">Authorization</span></span>|<span data-ttu-id="4f268-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4f268-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f268-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4f268-125">Accept</span></span>|<span data-ttu-id="4f268-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4f268-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f268-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4f268-127">Request body</span></span>
<span data-ttu-id="4f268-128">No corpo da solicitação, forneça uma representação JSON do objeto windowsAppX.</span><span class="sxs-lookup"><span data-stu-id="4f268-128">In the request body, supply a JSON representation for the windowsAppX object.</span></span>

<span data-ttu-id="4f268-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsAppX.</span><span class="sxs-lookup"><span data-stu-id="4f268-129">The following table shows the properties that are required when you create the windowsAppX.</span></span>

|<span data-ttu-id="4f268-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4f268-130">Property</span></span>|<span data-ttu-id="4f268-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4f268-131">Type</span></span>|<span data-ttu-id="4f268-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f268-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f268-133">id</span><span class="sxs-lookup"><span data-stu-id="4f268-133">id</span></span>|<span data-ttu-id="4f268-134">String</span><span class="sxs-lookup"><span data-stu-id="4f268-134">String</span></span>|<span data-ttu-id="4f268-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4f268-135">Key of the entity.</span></span> <span data-ttu-id="4f268-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4f268-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4f268-137">displayName</span><span class="sxs-lookup"><span data-stu-id="4f268-137">displayName</span></span>|<span data-ttu-id="4f268-138">String</span><span class="sxs-lookup"><span data-stu-id="4f268-138">String</span></span>|<span data-ttu-id="4f268-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="4f268-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="4f268-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4f268-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4f268-141">description</span><span class="sxs-lookup"><span data-stu-id="4f268-141">description</span></span>|<span data-ttu-id="4f268-142">String</span><span class="sxs-lookup"><span data-stu-id="4f268-142">String</span></span>|<span data-ttu-id="4f268-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4f268-143">The description of the app.</span></span> <span data-ttu-id="4f268-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4f268-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4f268-145">publicador</span><span class="sxs-lookup"><span data-stu-id="4f268-145">publisher</span></span>|<span data-ttu-id="4f268-146">String</span><span class="sxs-lookup"><span data-stu-id="4f268-146">String</span></span>|<span data-ttu-id="4f268-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4f268-147">The publisher of the app.</span></span> <span data-ttu-id="4f268-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4f268-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4f268-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="4f268-149">largeIcon</span></span>|[<span data-ttu-id="4f268-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="4f268-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="4f268-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="4f268-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="4f268-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4f268-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4f268-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4f268-153">createdDateTime</span></span>|<span data-ttu-id="4f268-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f268-154">DateTimeOffset</span></span>|<span data-ttu-id="4f268-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4f268-155">The date and time the app was created.</span></span> <span data-ttu-id="4f268-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4f268-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4f268-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4f268-157">lastModifiedDateTime</span></span>|<span data-ttu-id="4f268-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f268-158">DateTimeOffset</span></span>|<span data-ttu-id="4f268-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="4f268-159">The date and time the app was last modified.</span></span> <span data-ttu-id="4f268-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4f268-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4f268-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="4f268-161">isFeatured</span></span>|<span data-ttu-id="4f268-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f268-162">Boolean</span></span>|<span data-ttu-id="4f268-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4f268-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4f268-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="4f268-164">privacyInformationUrl</span></span>|<span data-ttu-id="4f268-165">String</span><span class="sxs-lookup"><span data-stu-id="4f268-165">String</span></span>|<span data-ttu-id="4f268-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="4f268-166">The privacy statement Url.</span></span> <span data-ttu-id="4f268-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4f268-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4f268-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="4f268-168">informationUrl</span></span>|<span data-ttu-id="4f268-169">String</span><span class="sxs-lookup"><span data-stu-id="4f268-169">String</span></span>|<span data-ttu-id="4f268-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="4f268-170">The more information Url.</span></span> <span data-ttu-id="4f268-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4f268-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4f268-172">proprietário</span><span class="sxs-lookup"><span data-stu-id="4f268-172">owner</span></span>|<span data-ttu-id="4f268-173">String</span><span class="sxs-lookup"><span data-stu-id="4f268-173">String</span></span>|<span data-ttu-id="4f268-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="4f268-174">The owner of the app.</span></span> <span data-ttu-id="4f268-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4f268-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4f268-176">developer</span><span class="sxs-lookup"><span data-stu-id="4f268-176">developer</span></span>|<span data-ttu-id="4f268-177">String</span><span class="sxs-lookup"><span data-stu-id="4f268-177">String</span></span>|<span data-ttu-id="4f268-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4f268-178">The developer of the app.</span></span> <span data-ttu-id="4f268-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4f268-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4f268-180">notes</span><span class="sxs-lookup"><span data-stu-id="4f268-180">notes</span></span>|<span data-ttu-id="4f268-181">String</span><span class="sxs-lookup"><span data-stu-id="4f268-181">String</span></span>|<span data-ttu-id="4f268-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4f268-182">Notes for the app.</span></span> <span data-ttu-id="4f268-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4f268-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4f268-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="4f268-184">uploadState</span></span>|<span data-ttu-id="4f268-185">Int32</span><span class="sxs-lookup"><span data-stu-id="4f268-185">Int32</span></span>|<span data-ttu-id="4f268-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="4f268-186">The upload state.</span></span> <span data-ttu-id="4f268-187">Os valores possíveis são: 0- `Not Ready` , 1- `Ready` , 2- `Processing` .</span><span class="sxs-lookup"><span data-stu-id="4f268-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="4f268-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4f268-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4f268-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="4f268-189">publishingState</span></span>|[<span data-ttu-id="4f268-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="4f268-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="4f268-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4f268-191">The publishing state for the app.</span></span> <span data-ttu-id="4f268-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="4f268-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="4f268-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4f268-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="4f268-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="4f268-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="4f268-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="4f268-195">isAssigned</span></span>|<span data-ttu-id="4f268-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f268-196">Boolean</span></span>|<span data-ttu-id="4f268-197">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="4f268-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="4f268-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4f268-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4f268-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4f268-199">roleScopeTagIds</span></span>|<span data-ttu-id="4f268-200">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="4f268-200">String collection</span></span>|<span data-ttu-id="4f268-201">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="4f268-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="4f268-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4f268-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4f268-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="4f268-203">dependentAppCount</span></span>|<span data-ttu-id="4f268-204">Int32</span><span class="sxs-lookup"><span data-stu-id="4f268-204">Int32</span></span>|<span data-ttu-id="4f268-205">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="4f268-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="4f268-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4f268-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4f268-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="4f268-207">supersedingAppCount</span></span>|<span data-ttu-id="4f268-208">Int32</span><span class="sxs-lookup"><span data-stu-id="4f268-208">Int32</span></span>|<span data-ttu-id="4f268-209">O número total de aplicativos que este aplicativo substitui direta ou indiretamente.</span><span class="sxs-lookup"><span data-stu-id="4f268-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="4f268-210">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4f268-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4f268-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="4f268-211">supersededAppCount</span></span>|<span data-ttu-id="4f268-212">Int32</span><span class="sxs-lookup"><span data-stu-id="4f268-212">Int32</span></span>|<span data-ttu-id="4f268-213">O número total de aplicativos que este aplicativo está substituindo direta ou indiretamente por.</span><span class="sxs-lookup"><span data-stu-id="4f268-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="4f268-214">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4f268-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4f268-215">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="4f268-215">committedContentVersion</span></span>|<span data-ttu-id="4f268-216">String</span><span class="sxs-lookup"><span data-stu-id="4f268-216">String</span></span>|<span data-ttu-id="4f268-217">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="4f268-217">The internal committed content version.</span></span> <span data-ttu-id="4f268-218">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="4f268-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="4f268-219">fileName</span><span class="sxs-lookup"><span data-stu-id="4f268-219">fileName</span></span>|<span data-ttu-id="4f268-220">String</span><span class="sxs-lookup"><span data-stu-id="4f268-220">String</span></span>|<span data-ttu-id="4f268-221">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="4f268-221">The name of the main Lob application file.</span></span> <span data-ttu-id="4f268-222">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="4f268-222">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="4f268-223">size</span><span class="sxs-lookup"><span data-stu-id="4f268-223">size</span></span>|<span data-ttu-id="4f268-224">Int64</span><span class="sxs-lookup"><span data-stu-id="4f268-224">Int64</span></span>|<span data-ttu-id="4f268-225">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="4f268-225">The total size, including all uploaded files.</span></span> <span data-ttu-id="4f268-226">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="4f268-226">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="4f268-227">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="4f268-227">applicableArchitectures</span></span>|[<span data-ttu-id="4f268-228">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="4f268-228">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="4f268-229">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="4f268-229">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="4f268-230">Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="4f268-230">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="4f268-231">identityName</span><span class="sxs-lookup"><span data-stu-id="4f268-231">identityName</span></span>|<span data-ttu-id="4f268-232">String</span><span class="sxs-lookup"><span data-stu-id="4f268-232">String</span></span>|<span data-ttu-id="4f268-233">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="4f268-233">The Identity Name.</span></span>|
|<span data-ttu-id="4f268-234">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="4f268-234">identityPublisherHash</span></span>|<span data-ttu-id="4f268-235">String</span><span class="sxs-lookup"><span data-stu-id="4f268-235">String</span></span>|<span data-ttu-id="4f268-236">O Hash do Publicador de Identidade.</span><span class="sxs-lookup"><span data-stu-id="4f268-236">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="4f268-237">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="4f268-237">identityResourceIdentifier</span></span>|<span data-ttu-id="4f268-238">String</span><span class="sxs-lookup"><span data-stu-id="4f268-238">String</span></span>|<span data-ttu-id="4f268-239">O Identificador de Recurso da Identidade.</span><span class="sxs-lookup"><span data-stu-id="4f268-239">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="4f268-240">isBundle</span><span class="sxs-lookup"><span data-stu-id="4f268-240">isBundle</span></span>|<span data-ttu-id="4f268-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f268-241">Boolean</span></span>|<span data-ttu-id="4f268-242">Se o aplicativo é um pacote ou não.</span><span class="sxs-lookup"><span data-stu-id="4f268-242">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="4f268-243">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="4f268-243">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="4f268-244">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="4f268-244">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="4f268-245">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="4f268-245">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="4f268-246">identityVersion</span><span class="sxs-lookup"><span data-stu-id="4f268-246">identityVersion</span></span>|<span data-ttu-id="4f268-247">String</span><span class="sxs-lookup"><span data-stu-id="4f268-247">String</span></span>|<span data-ttu-id="4f268-248">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="4f268-248">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="4f268-249">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f268-249">Response</span></span>
<span data-ttu-id="4f268-250">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windowsAppX](../resources/intune-apps-windowsappx.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4f268-250">If successful, this method returns a `201 Created` response code and a [windowsAppX](../resources/intune-apps-windowsappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f268-251">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4f268-251">Example</span></span>

### <a name="request"></a><span data-ttu-id="4f268-252">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4f268-252">Request</span></span>
<span data-ttu-id="4f268-253">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4f268-253">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="4f268-254">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f268-254">Response</span></span>
<span data-ttu-id="4f268-p125">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4f268-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






