---
title: Criar macOSMicrosoftEdgeApp
description: Criar um novo objeto macOSMicrosoftEdgeApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 95fabb65882a9838a5918b95af7e4ab6ec6d02af
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49251497"
---
# <a name="create-macosmicrosoftedgeapp"></a><span data-ttu-id="85852-103">Criar macOSMicrosoftEdgeApp</span><span class="sxs-lookup"><span data-stu-id="85852-103">Create macOSMicrosoftEdgeApp</span></span>

<span data-ttu-id="85852-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85852-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="85852-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="85852-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="85852-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="85852-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85852-107">Criar um novo objeto [macOSMicrosoftEdgeApp](../resources/intune-apps-macosmicrosoftedgeapp.md) .</span><span class="sxs-lookup"><span data-stu-id="85852-107">Create a new [macOSMicrosoftEdgeApp](../resources/intune-apps-macosmicrosoftedgeapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="85852-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="85852-108">Prerequisites</span></span>
<span data-ttu-id="85852-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85852-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85852-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="85852-111">Permission type</span></span>|<span data-ttu-id="85852-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="85852-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85852-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="85852-113">Delegated (work or school account)</span></span>|<span data-ttu-id="85852-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85852-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="85852-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="85852-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85852-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="85852-116">Not supported.</span></span>|
|<span data-ttu-id="85852-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="85852-117">Application</span></span>|<span data-ttu-id="85852-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85852-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="85852-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="85852-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="85852-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="85852-120">Request headers</span></span>
|<span data-ttu-id="85852-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="85852-121">Header</span></span>|<span data-ttu-id="85852-122">Valor</span><span class="sxs-lookup"><span data-stu-id="85852-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="85852-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="85852-123">Authorization</span></span>|<span data-ttu-id="85852-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="85852-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="85852-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="85852-125">Accept</span></span>|<span data-ttu-id="85852-126">application/json</span><span class="sxs-lookup"><span data-stu-id="85852-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="85852-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="85852-127">Request body</span></span>
<span data-ttu-id="85852-128">No corpo da solicitação, forneça uma representação JSON do objeto macOSMicrosoftEdgeApp.</span><span class="sxs-lookup"><span data-stu-id="85852-128">In the request body, supply a JSON representation for the macOSMicrosoftEdgeApp object.</span></span>

<span data-ttu-id="85852-129">A tabela a seguir mostra as propriedades que são necessárias ao criar macOSMicrosoftEdgeApp.</span><span class="sxs-lookup"><span data-stu-id="85852-129">The following table shows the properties that are required when you create the macOSMicrosoftEdgeApp.</span></span>

|<span data-ttu-id="85852-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="85852-130">Property</span></span>|<span data-ttu-id="85852-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="85852-131">Type</span></span>|<span data-ttu-id="85852-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="85852-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85852-133">id</span><span class="sxs-lookup"><span data-stu-id="85852-133">id</span></span>|<span data-ttu-id="85852-134">String</span><span class="sxs-lookup"><span data-stu-id="85852-134">String</span></span>|<span data-ttu-id="85852-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="85852-135">Key of the entity.</span></span> <span data-ttu-id="85852-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="85852-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="85852-137">displayName</span><span class="sxs-lookup"><span data-stu-id="85852-137">displayName</span></span>|<span data-ttu-id="85852-138">String</span><span class="sxs-lookup"><span data-stu-id="85852-138">String</span></span>|<span data-ttu-id="85852-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="85852-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="85852-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="85852-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="85852-141">description</span><span class="sxs-lookup"><span data-stu-id="85852-141">description</span></span>|<span data-ttu-id="85852-142">String</span><span class="sxs-lookup"><span data-stu-id="85852-142">String</span></span>|<span data-ttu-id="85852-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="85852-143">The description of the app.</span></span> <span data-ttu-id="85852-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="85852-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="85852-145">publicador</span><span class="sxs-lookup"><span data-stu-id="85852-145">publisher</span></span>|<span data-ttu-id="85852-146">String</span><span class="sxs-lookup"><span data-stu-id="85852-146">String</span></span>|<span data-ttu-id="85852-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="85852-147">The publisher of the app.</span></span> <span data-ttu-id="85852-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="85852-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="85852-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="85852-149">largeIcon</span></span>|[<span data-ttu-id="85852-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="85852-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="85852-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="85852-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="85852-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="85852-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="85852-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="85852-153">createdDateTime</span></span>|<span data-ttu-id="85852-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85852-154">DateTimeOffset</span></span>|<span data-ttu-id="85852-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="85852-155">The date and time the app was created.</span></span> <span data-ttu-id="85852-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="85852-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="85852-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="85852-157">lastModifiedDateTime</span></span>|<span data-ttu-id="85852-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85852-158">DateTimeOffset</span></span>|<span data-ttu-id="85852-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="85852-159">The date and time the app was last modified.</span></span> <span data-ttu-id="85852-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="85852-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="85852-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="85852-161">isFeatured</span></span>|<span data-ttu-id="85852-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="85852-162">Boolean</span></span>|<span data-ttu-id="85852-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="85852-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="85852-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="85852-164">privacyInformationUrl</span></span>|<span data-ttu-id="85852-165">String</span><span class="sxs-lookup"><span data-stu-id="85852-165">String</span></span>|<span data-ttu-id="85852-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="85852-166">The privacy statement Url.</span></span> <span data-ttu-id="85852-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="85852-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="85852-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="85852-168">informationUrl</span></span>|<span data-ttu-id="85852-169">String</span><span class="sxs-lookup"><span data-stu-id="85852-169">String</span></span>|<span data-ttu-id="85852-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="85852-170">The more information Url.</span></span> <span data-ttu-id="85852-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="85852-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="85852-172">owner</span><span class="sxs-lookup"><span data-stu-id="85852-172">owner</span></span>|<span data-ttu-id="85852-173">String</span><span class="sxs-lookup"><span data-stu-id="85852-173">String</span></span>|<span data-ttu-id="85852-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="85852-174">The owner of the app.</span></span> <span data-ttu-id="85852-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="85852-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="85852-176">developer</span><span class="sxs-lookup"><span data-stu-id="85852-176">developer</span></span>|<span data-ttu-id="85852-177">String</span><span class="sxs-lookup"><span data-stu-id="85852-177">String</span></span>|<span data-ttu-id="85852-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="85852-178">The developer of the app.</span></span> <span data-ttu-id="85852-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="85852-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="85852-180">notes</span><span class="sxs-lookup"><span data-stu-id="85852-180">notes</span></span>|<span data-ttu-id="85852-181">String</span><span class="sxs-lookup"><span data-stu-id="85852-181">String</span></span>|<span data-ttu-id="85852-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="85852-182">Notes for the app.</span></span> <span data-ttu-id="85852-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="85852-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="85852-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="85852-184">uploadState</span></span>|<span data-ttu-id="85852-185">Int32</span><span class="sxs-lookup"><span data-stu-id="85852-185">Int32</span></span>|<span data-ttu-id="85852-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="85852-186">The upload state.</span></span> <span data-ttu-id="85852-187">Os valores possíveis são: 0- `Not Ready` , 1- `Ready` , 2- `Processing` .</span><span class="sxs-lookup"><span data-stu-id="85852-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="85852-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="85852-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="85852-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="85852-189">publishingState</span></span>|[<span data-ttu-id="85852-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="85852-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="85852-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="85852-191">The publishing state for the app.</span></span> <span data-ttu-id="85852-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="85852-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="85852-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="85852-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="85852-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="85852-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="85852-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="85852-195">isAssigned</span></span>|<span data-ttu-id="85852-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="85852-196">Boolean</span></span>|<span data-ttu-id="85852-197">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="85852-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="85852-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="85852-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="85852-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="85852-199">roleScopeTagIds</span></span>|<span data-ttu-id="85852-200">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="85852-200">String collection</span></span>|<span data-ttu-id="85852-201">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="85852-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="85852-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="85852-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="85852-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="85852-203">dependentAppCount</span></span>|<span data-ttu-id="85852-204">Int32</span><span class="sxs-lookup"><span data-stu-id="85852-204">Int32</span></span>|<span data-ttu-id="85852-205">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="85852-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="85852-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="85852-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="85852-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="85852-207">supersedingAppCount</span></span>|<span data-ttu-id="85852-208">Int32</span><span class="sxs-lookup"><span data-stu-id="85852-208">Int32</span></span>|<span data-ttu-id="85852-209">O número total de aplicativos que este aplicativo substitui direta ou indiretamente.</span><span class="sxs-lookup"><span data-stu-id="85852-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="85852-210">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="85852-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="85852-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="85852-211">supersededAppCount</span></span>|<span data-ttu-id="85852-212">Int32</span><span class="sxs-lookup"><span data-stu-id="85852-212">Int32</span></span>|<span data-ttu-id="85852-213">O número total de aplicativos que este aplicativo está substituindo direta ou indiretamente por.</span><span class="sxs-lookup"><span data-stu-id="85852-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="85852-214">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="85852-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="85852-215">canal</span><span class="sxs-lookup"><span data-stu-id="85852-215">channel</span></span>|[<span data-ttu-id="85852-216">microsoftEdgeChannel</span><span class="sxs-lookup"><span data-stu-id="85852-216">microsoftEdgeChannel</span></span>](../resources/intune-apps-microsoftedgechannel.md)|<span data-ttu-id="85852-217">O canal a ser instalado nos dispositivos de destino.</span><span class="sxs-lookup"><span data-stu-id="85852-217">The channel to install on target devices.</span></span> <span data-ttu-id="85852-218">Os valores possíveis são: `dev`, `beta`, `stable`.</span><span class="sxs-lookup"><span data-stu-id="85852-218">Possible values are: `dev`, `beta`, `stable`.</span></span>|



## <a name="response"></a><span data-ttu-id="85852-219">Resposta</span><span class="sxs-lookup"><span data-stu-id="85852-219">Response</span></span>
<span data-ttu-id="85852-220">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [macOSMicrosoftEdgeApp](../resources/intune-apps-macosmicrosoftedgeapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="85852-220">If successful, this method returns a `201 Created` response code and a [macOSMicrosoftEdgeApp](../resources/intune-apps-macosmicrosoftedgeapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85852-221">Exemplo</span><span class="sxs-lookup"><span data-stu-id="85852-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="85852-222">Solicitação</span><span class="sxs-lookup"><span data-stu-id="85852-222">Request</span></span>
<span data-ttu-id="85852-223">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="85852-223">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 799

{
  "@odata.type": "#microsoft.graph.macOSMicrosoftEdgeApp",
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
  "channel": "beta"
}
```

### <a name="response"></a><span data-ttu-id="85852-224">Resposta</span><span class="sxs-lookup"><span data-stu-id="85852-224">Response</span></span>
<span data-ttu-id="85852-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="85852-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 971

{
  "@odata.type": "#microsoft.graph.macOSMicrosoftEdgeApp",
  "id": "c964092a-092a-c964-2a09-64c92a0964c9",
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
  "channel": "beta"
}
```




