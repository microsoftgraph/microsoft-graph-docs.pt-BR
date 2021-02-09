---
title: Criar androidStoreApp
description: Criar um novo objeto androidStoreApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c5d03ffc0585572496f10aaffd4d6bdc41a570b9
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157439"
---
# <a name="create-androidstoreapp"></a><span data-ttu-id="61f62-103">Criar androidStoreApp</span><span class="sxs-lookup"><span data-stu-id="61f62-103">Create androidStoreApp</span></span>

<span data-ttu-id="61f62-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61f62-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="61f62-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="61f62-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="61f62-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="61f62-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61f62-107">Criar um novo objeto [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="61f62-107">Create a new [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="61f62-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="61f62-108">Prerequisites</span></span>
<span data-ttu-id="61f62-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61f62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61f62-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="61f62-111">Permission type</span></span>|<span data-ttu-id="61f62-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="61f62-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="61f62-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="61f62-113">Delegated (work or school account)</span></span>|<span data-ttu-id="61f62-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61f62-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="61f62-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="61f62-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="61f62-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="61f62-116">Not supported.</span></span>|
|<span data-ttu-id="61f62-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="61f62-117">Application</span></span>|<span data-ttu-id="61f62-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61f62-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="61f62-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="61f62-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="61f62-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="61f62-120">Request headers</span></span>
|<span data-ttu-id="61f62-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="61f62-121">Header</span></span>|<span data-ttu-id="61f62-122">Valor</span><span class="sxs-lookup"><span data-stu-id="61f62-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="61f62-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="61f62-123">Authorization</span></span>|<span data-ttu-id="61f62-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="61f62-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="61f62-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="61f62-125">Accept</span></span>|<span data-ttu-id="61f62-126">application/json</span><span class="sxs-lookup"><span data-stu-id="61f62-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="61f62-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="61f62-127">Request body</span></span>
<span data-ttu-id="61f62-128">No corpo da solicitação, forneça uma representação JSON do objeto androidStoreApp.</span><span class="sxs-lookup"><span data-stu-id="61f62-128">In the request body, supply a JSON representation for the androidStoreApp object.</span></span>

<span data-ttu-id="61f62-129">A tabela a seguir mostra as propriedades que são necessárias ao criar androidStoreApp.</span><span class="sxs-lookup"><span data-stu-id="61f62-129">The following table shows the properties that are required when you create the androidStoreApp.</span></span>

|<span data-ttu-id="61f62-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="61f62-130">Property</span></span>|<span data-ttu-id="61f62-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="61f62-131">Type</span></span>|<span data-ttu-id="61f62-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="61f62-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61f62-133">id</span><span class="sxs-lookup"><span data-stu-id="61f62-133">id</span></span>|<span data-ttu-id="61f62-134">String</span><span class="sxs-lookup"><span data-stu-id="61f62-134">String</span></span>|<span data-ttu-id="61f62-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="61f62-135">Key of the entity.</span></span> <span data-ttu-id="61f62-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="61f62-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="61f62-137">displayName</span><span class="sxs-lookup"><span data-stu-id="61f62-137">displayName</span></span>|<span data-ttu-id="61f62-138">String</span><span class="sxs-lookup"><span data-stu-id="61f62-138">String</span></span>|<span data-ttu-id="61f62-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="61f62-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="61f62-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="61f62-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="61f62-141">description</span><span class="sxs-lookup"><span data-stu-id="61f62-141">description</span></span>|<span data-ttu-id="61f62-142">String</span><span class="sxs-lookup"><span data-stu-id="61f62-142">String</span></span>|<span data-ttu-id="61f62-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="61f62-143">The description of the app.</span></span> <span data-ttu-id="61f62-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="61f62-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="61f62-145">publicador</span><span class="sxs-lookup"><span data-stu-id="61f62-145">publisher</span></span>|<span data-ttu-id="61f62-146">String</span><span class="sxs-lookup"><span data-stu-id="61f62-146">String</span></span>|<span data-ttu-id="61f62-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="61f62-147">The publisher of the app.</span></span> <span data-ttu-id="61f62-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="61f62-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="61f62-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="61f62-149">largeIcon</span></span>|[<span data-ttu-id="61f62-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="61f62-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="61f62-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="61f62-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="61f62-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="61f62-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="61f62-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="61f62-153">createdDateTime</span></span>|<span data-ttu-id="61f62-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61f62-154">DateTimeOffset</span></span>|<span data-ttu-id="61f62-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="61f62-155">The date and time the app was created.</span></span> <span data-ttu-id="61f62-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="61f62-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="61f62-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="61f62-157">lastModifiedDateTime</span></span>|<span data-ttu-id="61f62-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61f62-158">DateTimeOffset</span></span>|<span data-ttu-id="61f62-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="61f62-159">The date and time the app was last modified.</span></span> <span data-ttu-id="61f62-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="61f62-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="61f62-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="61f62-161">isFeatured</span></span>|<span data-ttu-id="61f62-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="61f62-162">Boolean</span></span>|<span data-ttu-id="61f62-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="61f62-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="61f62-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="61f62-164">privacyInformationUrl</span></span>|<span data-ttu-id="61f62-165">String</span><span class="sxs-lookup"><span data-stu-id="61f62-165">String</span></span>|<span data-ttu-id="61f62-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="61f62-166">The privacy statement Url.</span></span> <span data-ttu-id="61f62-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="61f62-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="61f62-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="61f62-168">informationUrl</span></span>|<span data-ttu-id="61f62-169">String</span><span class="sxs-lookup"><span data-stu-id="61f62-169">String</span></span>|<span data-ttu-id="61f62-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="61f62-170">The more information Url.</span></span> <span data-ttu-id="61f62-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="61f62-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="61f62-172">owner</span><span class="sxs-lookup"><span data-stu-id="61f62-172">owner</span></span>|<span data-ttu-id="61f62-173">String</span><span class="sxs-lookup"><span data-stu-id="61f62-173">String</span></span>|<span data-ttu-id="61f62-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="61f62-174">The owner of the app.</span></span> <span data-ttu-id="61f62-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="61f62-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="61f62-176">developer</span><span class="sxs-lookup"><span data-stu-id="61f62-176">developer</span></span>|<span data-ttu-id="61f62-177">String</span><span class="sxs-lookup"><span data-stu-id="61f62-177">String</span></span>|<span data-ttu-id="61f62-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="61f62-178">The developer of the app.</span></span> <span data-ttu-id="61f62-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="61f62-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="61f62-180">notes</span><span class="sxs-lookup"><span data-stu-id="61f62-180">notes</span></span>|<span data-ttu-id="61f62-181">String</span><span class="sxs-lookup"><span data-stu-id="61f62-181">String</span></span>|<span data-ttu-id="61f62-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="61f62-182">Notes for the app.</span></span> <span data-ttu-id="61f62-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="61f62-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="61f62-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="61f62-184">uploadState</span></span>|<span data-ttu-id="61f62-185">Int32</span><span class="sxs-lookup"><span data-stu-id="61f62-185">Int32</span></span>|<span data-ttu-id="61f62-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="61f62-186">The upload state.</span></span> <span data-ttu-id="61f62-187">Os valores possíveis são: 0 - `Not Ready` , 1 - `Ready` , 2 - `Processing` .</span><span class="sxs-lookup"><span data-stu-id="61f62-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="61f62-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="61f62-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="61f62-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="61f62-189">publishingState</span></span>|[<span data-ttu-id="61f62-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="61f62-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="61f62-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="61f62-191">The publishing state for the app.</span></span> <span data-ttu-id="61f62-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="61f62-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="61f62-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="61f62-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="61f62-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="61f62-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="61f62-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="61f62-195">isAssigned</span></span>|<span data-ttu-id="61f62-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="61f62-196">Boolean</span></span>|<span data-ttu-id="61f62-197">O valor que indica se o aplicativo está atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="61f62-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="61f62-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="61f62-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="61f62-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="61f62-199">roleScopeTagIds</span></span>|<span data-ttu-id="61f62-200">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="61f62-200">String collection</span></span>|<span data-ttu-id="61f62-201">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="61f62-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="61f62-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="61f62-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="61f62-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="61f62-203">dependentAppCount</span></span>|<span data-ttu-id="61f62-204">Int32</span><span class="sxs-lookup"><span data-stu-id="61f62-204">Int32</span></span>|<span data-ttu-id="61f62-205">O número total de dependências que o aplicativo filho tem.</span><span class="sxs-lookup"><span data-stu-id="61f62-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="61f62-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="61f62-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="61f62-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="61f62-207">supersedingAppCount</span></span>|<span data-ttu-id="61f62-208">Int32</span><span class="sxs-lookup"><span data-stu-id="61f62-208">Int32</span></span>|<span data-ttu-id="61f62-209">O número total de aplicativos que este aplicativo é direta ou indiretamente é supersedido.</span><span class="sxs-lookup"><span data-stu-id="61f62-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="61f62-210">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="61f62-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="61f62-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="61f62-211">supersededAppCount</span></span>|<span data-ttu-id="61f62-212">Int32</span><span class="sxs-lookup"><span data-stu-id="61f62-212">Int32</span></span>|<span data-ttu-id="61f62-213">O número total de aplicativos pelos quais esse aplicativo é direta ou indiretamente sobressu valorado.</span><span class="sxs-lookup"><span data-stu-id="61f62-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="61f62-214">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="61f62-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="61f62-215">packageId</span><span class="sxs-lookup"><span data-stu-id="61f62-215">packageId</span></span>|<span data-ttu-id="61f62-216">String</span><span class="sxs-lookup"><span data-stu-id="61f62-216">String</span></span>|<span data-ttu-id="61f62-217">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="61f62-217">The package identifier.</span></span>|
|<span data-ttu-id="61f62-218">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="61f62-218">appIdentifier</span></span>|<span data-ttu-id="61f62-219">String</span><span class="sxs-lookup"><span data-stu-id="61f62-219">String</span></span>|<span data-ttu-id="61f62-220">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="61f62-220">The Identity Name.</span></span>|
|<span data-ttu-id="61f62-221">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="61f62-221">appStoreUrl</span></span>|<span data-ttu-id="61f62-222">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="61f62-222">String</span></span>|<span data-ttu-id="61f62-223">A URL da loja de aplicativos Android.</span><span class="sxs-lookup"><span data-stu-id="61f62-223">The Android app store URL.</span></span>|
|<span data-ttu-id="61f62-224">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="61f62-224">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="61f62-225">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="61f62-225">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="61f62-226">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="61f62-226">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="61f62-227">Resposta</span><span class="sxs-lookup"><span data-stu-id="61f62-227">Response</span></span>
<span data-ttu-id="61f62-228">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [androidStoreApp](../resources/intune-apps-androidstoreapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="61f62-228">If successful, this method returns a `201 Created` response code and a [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61f62-229">Exemplo</span><span class="sxs-lookup"><span data-stu-id="61f62-229">Example</span></span>

### <a name="request"></a><span data-ttu-id="61f62-230">Solicitação</span><span class="sxs-lookup"><span data-stu-id="61f62-230">Request</span></span>
<span data-ttu-id="61f62-231">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="61f62-231">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1327

{
  "@odata.type": "#microsoft.graph.androidStoreApp",
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
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
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
  }
}
```

### <a name="response"></a><span data-ttu-id="61f62-232">Resposta</span><span class="sxs-lookup"><span data-stu-id="61f62-232">Response</span></span>
<span data-ttu-id="61f62-p121">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="61f62-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1499

{
  "@odata.type": "#microsoft.graph.androidStoreApp",
  "id": "1f2b7654-7654-1f2b-5476-2b1f54762b1f",
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
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
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
  }
}
```




