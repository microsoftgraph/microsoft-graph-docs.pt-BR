---
title: Criar windowsStoreApp
description: Crie um novo objeto windowsStoreApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e378420c8d8c4a9e13d1bf53559105f0fdde49fb
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51133343"
---
# <a name="create-windowsstoreapp"></a><span data-ttu-id="bbf1f-103">Criar windowsStoreApp</span><span class="sxs-lookup"><span data-stu-id="bbf1f-103">Create windowsStoreApp</span></span>

<span data-ttu-id="bbf1f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bbf1f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bbf1f-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bbf1f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bbf1f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bbf1f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bbf1f-107">Crie um novo [objeto windowsStoreApp.](../resources/intune-apps-windowsstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="bbf1f-107">Create a new [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bbf1f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bbf1f-108">Prerequisites</span></span>
<span data-ttu-id="bbf1f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bbf1f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bbf1f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bbf1f-111">Permission type</span></span>|<span data-ttu-id="bbf1f-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bbf1f-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bbf1f-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bbf1f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bbf1f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbf1f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bbf1f-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bbf1f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bbf1f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bbf1f-116">Not supported.</span></span>|
|<span data-ttu-id="bbf1f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bbf1f-117">Application</span></span>|<span data-ttu-id="bbf1f-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbf1f-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bbf1f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bbf1f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="bbf1f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bbf1f-120">Request headers</span></span>
|<span data-ttu-id="bbf1f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bbf1f-121">Header</span></span>|<span data-ttu-id="bbf1f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="bbf1f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bbf1f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bbf1f-123">Authorization</span></span>|<span data-ttu-id="bbf1f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bbf1f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bbf1f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bbf1f-125">Accept</span></span>|<span data-ttu-id="bbf1f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bbf1f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bbf1f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bbf1f-127">Request body</span></span>
<span data-ttu-id="bbf1f-128">No corpo da solicitação, fornece uma representação JSON para o objeto windowsStoreApp.</span><span class="sxs-lookup"><span data-stu-id="bbf1f-128">In the request body, supply a JSON representation for the windowsStoreApp object.</span></span>

<span data-ttu-id="bbf1f-129">A tabela a seguir mostra as propriedades necessárias ao criar o windowsStoreApp.</span><span class="sxs-lookup"><span data-stu-id="bbf1f-129">The following table shows the properties that are required when you create the windowsStoreApp.</span></span>

|<span data-ttu-id="bbf1f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bbf1f-130">Property</span></span>|<span data-ttu-id="bbf1f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="bbf1f-131">Type</span></span>|<span data-ttu-id="bbf1f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="bbf1f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bbf1f-133">id</span><span class="sxs-lookup"><span data-stu-id="bbf1f-133">id</span></span>|<span data-ttu-id="bbf1f-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bbf1f-134">String</span></span>|<span data-ttu-id="bbf1f-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="bbf1f-135">Key of the entity.</span></span> <span data-ttu-id="bbf1f-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bbf1f-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bbf1f-137">displayName</span><span class="sxs-lookup"><span data-stu-id="bbf1f-137">displayName</span></span>|<span data-ttu-id="bbf1f-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bbf1f-138">String</span></span>|<span data-ttu-id="bbf1f-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="bbf1f-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="bbf1f-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bbf1f-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bbf1f-141">descrição</span><span class="sxs-lookup"><span data-stu-id="bbf1f-141">description</span></span>|<span data-ttu-id="bbf1f-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bbf1f-142">String</span></span>|<span data-ttu-id="bbf1f-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bbf1f-143">The description of the app.</span></span> <span data-ttu-id="bbf1f-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bbf1f-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bbf1f-145">publicador</span><span class="sxs-lookup"><span data-stu-id="bbf1f-145">publisher</span></span>|<span data-ttu-id="bbf1f-146">String</span><span class="sxs-lookup"><span data-stu-id="bbf1f-146">String</span></span>|<span data-ttu-id="bbf1f-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bbf1f-147">The publisher of the app.</span></span> <span data-ttu-id="bbf1f-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bbf1f-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bbf1f-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="bbf1f-149">largeIcon</span></span>|[<span data-ttu-id="bbf1f-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="bbf1f-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="bbf1f-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="bbf1f-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="bbf1f-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bbf1f-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bbf1f-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bbf1f-153">createdDateTime</span></span>|<span data-ttu-id="bbf1f-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bbf1f-154">DateTimeOffset</span></span>|<span data-ttu-id="bbf1f-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bbf1f-155">The date and time the app was created.</span></span> <span data-ttu-id="bbf1f-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bbf1f-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bbf1f-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bbf1f-157">lastModifiedDateTime</span></span>|<span data-ttu-id="bbf1f-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bbf1f-158">DateTimeOffset</span></span>|<span data-ttu-id="bbf1f-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="bbf1f-159">The date and time the app was last modified.</span></span> <span data-ttu-id="bbf1f-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bbf1f-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bbf1f-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="bbf1f-161">isFeatured</span></span>|<span data-ttu-id="bbf1f-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="bbf1f-162">Boolean</span></span>|<span data-ttu-id="bbf1f-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bbf1f-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bbf1f-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="bbf1f-164">privacyInformationUrl</span></span>|<span data-ttu-id="bbf1f-165">String</span><span class="sxs-lookup"><span data-stu-id="bbf1f-165">String</span></span>|<span data-ttu-id="bbf1f-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="bbf1f-166">The privacy statement Url.</span></span> <span data-ttu-id="bbf1f-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bbf1f-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bbf1f-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="bbf1f-168">informationUrl</span></span>|<span data-ttu-id="bbf1f-169">String</span><span class="sxs-lookup"><span data-stu-id="bbf1f-169">String</span></span>|<span data-ttu-id="bbf1f-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="bbf1f-170">The more information Url.</span></span> <span data-ttu-id="bbf1f-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bbf1f-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bbf1f-172">owner</span><span class="sxs-lookup"><span data-stu-id="bbf1f-172">owner</span></span>|<span data-ttu-id="bbf1f-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bbf1f-173">String</span></span>|<span data-ttu-id="bbf1f-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="bbf1f-174">The owner of the app.</span></span> <span data-ttu-id="bbf1f-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bbf1f-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bbf1f-176">developer</span><span class="sxs-lookup"><span data-stu-id="bbf1f-176">developer</span></span>|<span data-ttu-id="bbf1f-177">String</span><span class="sxs-lookup"><span data-stu-id="bbf1f-177">String</span></span>|<span data-ttu-id="bbf1f-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bbf1f-178">The developer of the app.</span></span> <span data-ttu-id="bbf1f-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bbf1f-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bbf1f-180">notes</span><span class="sxs-lookup"><span data-stu-id="bbf1f-180">notes</span></span>|<span data-ttu-id="bbf1f-181">String</span><span class="sxs-lookup"><span data-stu-id="bbf1f-181">String</span></span>|<span data-ttu-id="bbf1f-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bbf1f-182">Notes for the app.</span></span> <span data-ttu-id="bbf1f-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bbf1f-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bbf1f-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="bbf1f-184">uploadState</span></span>|<span data-ttu-id="bbf1f-185">Int32</span><span class="sxs-lookup"><span data-stu-id="bbf1f-185">Int32</span></span>|<span data-ttu-id="bbf1f-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="bbf1f-186">The upload state.</span></span> <span data-ttu-id="bbf1f-187">Os valores possíveis são: 0 - `Not Ready` , 1 - `Ready` , 2 - `Processing` .</span><span class="sxs-lookup"><span data-stu-id="bbf1f-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="bbf1f-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bbf1f-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bbf1f-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="bbf1f-189">publishingState</span></span>|[<span data-ttu-id="bbf1f-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="bbf1f-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="bbf1f-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bbf1f-191">The publishing state for the app.</span></span> <span data-ttu-id="bbf1f-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="bbf1f-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="bbf1f-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bbf1f-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="bbf1f-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="bbf1f-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="bbf1f-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="bbf1f-195">isAssigned</span></span>|<span data-ttu-id="bbf1f-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="bbf1f-196">Boolean</span></span>|<span data-ttu-id="bbf1f-197">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="bbf1f-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="bbf1f-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bbf1f-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bbf1f-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bbf1f-199">roleScopeTagIds</span></span>|<span data-ttu-id="bbf1f-200">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="bbf1f-200">String collection</span></span>|<span data-ttu-id="bbf1f-201">Lista de ids de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="bbf1f-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="bbf1f-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bbf1f-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bbf1f-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="bbf1f-203">dependentAppCount</span></span>|<span data-ttu-id="bbf1f-204">Int32</span><span class="sxs-lookup"><span data-stu-id="bbf1f-204">Int32</span></span>|<span data-ttu-id="bbf1f-205">O número total de dependências que o aplicativo filho tem.</span><span class="sxs-lookup"><span data-stu-id="bbf1f-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="bbf1f-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bbf1f-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bbf1f-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="bbf1f-207">supersedingAppCount</span></span>|<span data-ttu-id="bbf1f-208">Int32</span><span class="sxs-lookup"><span data-stu-id="bbf1f-208">Int32</span></span>|<span data-ttu-id="bbf1f-209">O número total de aplicativos que esse aplicativo sobressede direta ou indiretamente.</span><span class="sxs-lookup"><span data-stu-id="bbf1f-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="bbf1f-210">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bbf1f-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bbf1f-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="bbf1f-211">supersededAppCount</span></span>|<span data-ttu-id="bbf1f-212">Int32</span><span class="sxs-lookup"><span data-stu-id="bbf1f-212">Int32</span></span>|<span data-ttu-id="bbf1f-213">O número total de aplicativos pelos quais esse aplicativo é, direta ou indiretamente, é suplido.</span><span class="sxs-lookup"><span data-stu-id="bbf1f-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="bbf1f-214">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bbf1f-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bbf1f-215">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="bbf1f-215">appStoreUrl</span></span>|<span data-ttu-id="bbf1f-216">String</span><span class="sxs-lookup"><span data-stu-id="bbf1f-216">String</span></span>|<span data-ttu-id="bbf1f-217">A URL da Loja de Aplicativos do Windows.</span><span class="sxs-lookup"><span data-stu-id="bbf1f-217">The Windows app store URL.</span></span>|



## <a name="response"></a><span data-ttu-id="bbf1f-218">Resposta</span><span class="sxs-lookup"><span data-stu-id="bbf1f-218">Response</span></span>
<span data-ttu-id="bbf1f-219">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bbf1f-219">If successful, this method returns a `201 Created` response code and a [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bbf1f-220">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bbf1f-220">Example</span></span>

### <a name="request"></a><span data-ttu-id="bbf1f-221">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bbf1f-221">Request</span></span>
<span data-ttu-id="bbf1f-222">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bbf1f-222">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 825

{
  "@odata.type": "#microsoft.graph.windowsStoreApp",
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
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```

### <a name="response"></a><span data-ttu-id="bbf1f-223">Resposta</span><span class="sxs-lookup"><span data-stu-id="bbf1f-223">Response</span></span>
<span data-ttu-id="bbf1f-p121">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bbf1f-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 997

{
  "@odata.type": "#microsoft.graph.windowsStoreApp",
  "id": "fd4a5f8a-5f8a-fd4a-8a5f-4afd8a5f4afd",
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
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```




