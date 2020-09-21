---
title: Criar webApp
description: Cria um novo objeto webApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 03608db7af07ebd468e5ea062f672aeed6b5796a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47976792"
---
# <a name="create-webapp"></a><span data-ttu-id="478d8-103">Criar webApp</span><span class="sxs-lookup"><span data-stu-id="478d8-103">Create webApp</span></span>

<span data-ttu-id="478d8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="478d8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="478d8-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="478d8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="478d8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="478d8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="478d8-107">Cria um novo objeto [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="478d8-107">Create a new [webApp](../resources/intune-apps-webapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="478d8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="478d8-108">Prerequisites</span></span>
<span data-ttu-id="478d8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="478d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="478d8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="478d8-111">Permission type</span></span>|<span data-ttu-id="478d8-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="478d8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="478d8-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="478d8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="478d8-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="478d8-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="478d8-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="478d8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="478d8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="478d8-116">Not supported.</span></span>|
|<span data-ttu-id="478d8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="478d8-117">Application</span></span>|<span data-ttu-id="478d8-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="478d8-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="478d8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="478d8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="478d8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="478d8-120">Request headers</span></span>
|<span data-ttu-id="478d8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="478d8-121">Header</span></span>|<span data-ttu-id="478d8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="478d8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="478d8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="478d8-123">Authorization</span></span>|<span data-ttu-id="478d8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="478d8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="478d8-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="478d8-125">Accept</span></span>|<span data-ttu-id="478d8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="478d8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="478d8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="478d8-127">Request body</span></span>
<span data-ttu-id="478d8-128">No corpo da solicitação, forneça uma representação JSON do objeto webApp.</span><span class="sxs-lookup"><span data-stu-id="478d8-128">In the request body, supply a JSON representation for the webApp object.</span></span>

<span data-ttu-id="478d8-129">A tabela a seguir mostra as propriedades obrigatórias ao criar o webApp.</span><span class="sxs-lookup"><span data-stu-id="478d8-129">The following table shows the properties that are required when you create the webApp.</span></span>

|<span data-ttu-id="478d8-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="478d8-130">Property</span></span>|<span data-ttu-id="478d8-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="478d8-131">Type</span></span>|<span data-ttu-id="478d8-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="478d8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="478d8-133">id</span><span class="sxs-lookup"><span data-stu-id="478d8-133">id</span></span>|<span data-ttu-id="478d8-134">String</span><span class="sxs-lookup"><span data-stu-id="478d8-134">String</span></span>|<span data-ttu-id="478d8-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="478d8-135">Key of the entity.</span></span> <span data-ttu-id="478d8-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="478d8-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="478d8-137">displayName</span><span class="sxs-lookup"><span data-stu-id="478d8-137">displayName</span></span>|<span data-ttu-id="478d8-138">String</span><span class="sxs-lookup"><span data-stu-id="478d8-138">String</span></span>|<span data-ttu-id="478d8-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="478d8-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="478d8-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="478d8-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="478d8-141">description</span><span class="sxs-lookup"><span data-stu-id="478d8-141">description</span></span>|<span data-ttu-id="478d8-142">String</span><span class="sxs-lookup"><span data-stu-id="478d8-142">String</span></span>|<span data-ttu-id="478d8-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="478d8-143">The description of the app.</span></span> <span data-ttu-id="478d8-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="478d8-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="478d8-145">publicador</span><span class="sxs-lookup"><span data-stu-id="478d8-145">publisher</span></span>|<span data-ttu-id="478d8-146">String</span><span class="sxs-lookup"><span data-stu-id="478d8-146">String</span></span>|<span data-ttu-id="478d8-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="478d8-147">The publisher of the app.</span></span> <span data-ttu-id="478d8-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="478d8-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="478d8-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="478d8-149">largeIcon</span></span>|[<span data-ttu-id="478d8-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="478d8-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="478d8-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="478d8-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="478d8-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="478d8-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="478d8-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="478d8-153">createdDateTime</span></span>|<span data-ttu-id="478d8-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="478d8-154">DateTimeOffset</span></span>|<span data-ttu-id="478d8-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="478d8-155">The date and time the app was created.</span></span> <span data-ttu-id="478d8-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="478d8-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="478d8-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="478d8-157">lastModifiedDateTime</span></span>|<span data-ttu-id="478d8-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="478d8-158">DateTimeOffset</span></span>|<span data-ttu-id="478d8-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="478d8-159">The date and time the app was last modified.</span></span> <span data-ttu-id="478d8-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="478d8-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="478d8-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="478d8-161">isFeatured</span></span>|<span data-ttu-id="478d8-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="478d8-162">Boolean</span></span>|<span data-ttu-id="478d8-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="478d8-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="478d8-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="478d8-164">privacyInformationUrl</span></span>|<span data-ttu-id="478d8-165">String</span><span class="sxs-lookup"><span data-stu-id="478d8-165">String</span></span>|<span data-ttu-id="478d8-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="478d8-166">The privacy statement Url.</span></span> <span data-ttu-id="478d8-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="478d8-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="478d8-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="478d8-168">informationUrl</span></span>|<span data-ttu-id="478d8-169">String</span><span class="sxs-lookup"><span data-stu-id="478d8-169">String</span></span>|<span data-ttu-id="478d8-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="478d8-170">The more information Url.</span></span> <span data-ttu-id="478d8-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="478d8-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="478d8-172">proprietário</span><span class="sxs-lookup"><span data-stu-id="478d8-172">owner</span></span>|<span data-ttu-id="478d8-173">String</span><span class="sxs-lookup"><span data-stu-id="478d8-173">String</span></span>|<span data-ttu-id="478d8-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="478d8-174">The owner of the app.</span></span> <span data-ttu-id="478d8-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="478d8-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="478d8-176">developer</span><span class="sxs-lookup"><span data-stu-id="478d8-176">developer</span></span>|<span data-ttu-id="478d8-177">String</span><span class="sxs-lookup"><span data-stu-id="478d8-177">String</span></span>|<span data-ttu-id="478d8-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="478d8-178">The developer of the app.</span></span> <span data-ttu-id="478d8-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="478d8-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="478d8-180">notes</span><span class="sxs-lookup"><span data-stu-id="478d8-180">notes</span></span>|<span data-ttu-id="478d8-181">String</span><span class="sxs-lookup"><span data-stu-id="478d8-181">String</span></span>|<span data-ttu-id="478d8-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="478d8-182">Notes for the app.</span></span> <span data-ttu-id="478d8-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="478d8-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="478d8-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="478d8-184">uploadState</span></span>|<span data-ttu-id="478d8-185">Int32</span><span class="sxs-lookup"><span data-stu-id="478d8-185">Int32</span></span>|<span data-ttu-id="478d8-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="478d8-186">The upload state.</span></span> <span data-ttu-id="478d8-187">Os valores possíveis são: 0- `Not Ready` , 1- `Ready` , 2- `Processing` .</span><span class="sxs-lookup"><span data-stu-id="478d8-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="478d8-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="478d8-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="478d8-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="478d8-189">publishingState</span></span>|[<span data-ttu-id="478d8-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="478d8-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="478d8-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="478d8-191">The publishing state for the app.</span></span> <span data-ttu-id="478d8-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="478d8-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="478d8-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="478d8-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="478d8-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="478d8-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="478d8-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="478d8-195">isAssigned</span></span>|<span data-ttu-id="478d8-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="478d8-196">Boolean</span></span>|<span data-ttu-id="478d8-197">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="478d8-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="478d8-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="478d8-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="478d8-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="478d8-199">roleScopeTagIds</span></span>|<span data-ttu-id="478d8-200">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="478d8-200">String collection</span></span>|<span data-ttu-id="478d8-201">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="478d8-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="478d8-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="478d8-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="478d8-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="478d8-203">dependentAppCount</span></span>|<span data-ttu-id="478d8-204">Int32</span><span class="sxs-lookup"><span data-stu-id="478d8-204">Int32</span></span>|<span data-ttu-id="478d8-205">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="478d8-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="478d8-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="478d8-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="478d8-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="478d8-207">supersedingAppCount</span></span>|<span data-ttu-id="478d8-208">Int32</span><span class="sxs-lookup"><span data-stu-id="478d8-208">Int32</span></span>|<span data-ttu-id="478d8-209">O número total de aplicativos que este aplicativo substitui direta ou indiretamente.</span><span class="sxs-lookup"><span data-stu-id="478d8-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="478d8-210">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="478d8-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="478d8-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="478d8-211">supersededAppCount</span></span>|<span data-ttu-id="478d8-212">Int32</span><span class="sxs-lookup"><span data-stu-id="478d8-212">Int32</span></span>|<span data-ttu-id="478d8-213">O número total de aplicativos que este aplicativo está substituindo direta ou indiretamente por.</span><span class="sxs-lookup"><span data-stu-id="478d8-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="478d8-214">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="478d8-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="478d8-215">appUrl</span><span class="sxs-lookup"><span data-stu-id="478d8-215">appUrl</span></span>|<span data-ttu-id="478d8-216">String</span><span class="sxs-lookup"><span data-stu-id="478d8-216">String</span></span>|<span data-ttu-id="478d8-217">A URL do aplicativo Web.</span><span class="sxs-lookup"><span data-stu-id="478d8-217">The web app URL.</span></span>|
|<span data-ttu-id="478d8-218">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="478d8-218">useManagedBrowser</span></span>|<span data-ttu-id="478d8-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="478d8-219">Boolean</span></span>|<span data-ttu-id="478d8-220">Se o navegador gerenciado deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="478d8-220">Whether or not to use managed browser.</span></span> <span data-ttu-id="478d8-221">Essa propriedade só é aplicável ao Android e ao IOS.</span><span class="sxs-lookup"><span data-stu-id="478d8-221">This property is only applicable for Android and IOS.</span></span>|



## <a name="response"></a><span data-ttu-id="478d8-222">Resposta</span><span class="sxs-lookup"><span data-stu-id="478d8-222">Response</span></span>
<span data-ttu-id="478d8-223">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [webApp](../resources/intune-apps-webapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="478d8-223">If successful, this method returns a `201 Created` response code and a [webApp](../resources/intune-apps-webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="478d8-224">Exemplo</span><span class="sxs-lookup"><span data-stu-id="478d8-224">Example</span></span>

### <a name="request"></a><span data-ttu-id="478d8-225">Solicitação</span><span class="sxs-lookup"><span data-stu-id="478d8-225">Request</span></span>
<span data-ttu-id="478d8-226">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="478d8-226">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 836

{
  "@odata.type": "#microsoft.graph.webApp",
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
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```

### <a name="response"></a><span data-ttu-id="478d8-227">Resposta</span><span class="sxs-lookup"><span data-stu-id="478d8-227">Response</span></span>
<span data-ttu-id="478d8-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="478d8-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1008

{
  "@odata.type": "#microsoft.graph.webApp",
  "id": "4bdc5d30-5d30-4bdc-305d-dc4b305ddc4b",
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
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```






