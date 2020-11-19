---
title: Criar androidForWorkApp
description: Criar um novo objeto androidForWorkApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 40745c2ad8177d5ce6caa417591e83aa23688a7e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49254123"
---
# <a name="create-androidforworkapp"></a><span data-ttu-id="0f734-103">Criar androidForWorkApp</span><span class="sxs-lookup"><span data-stu-id="0f734-103">Create androidForWorkApp</span></span>

<span data-ttu-id="0f734-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f734-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0f734-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0f734-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0f734-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0f734-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f734-107">Criar um novo objeto [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) .</span><span class="sxs-lookup"><span data-stu-id="0f734-107">Create a new [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0f734-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0f734-108">Prerequisites</span></span>
<span data-ttu-id="0f734-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f734-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f734-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0f734-111">Permission type</span></span>|<span data-ttu-id="0f734-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0f734-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0f734-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0f734-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0f734-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f734-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0f734-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0f734-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0f734-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0f734-116">Not supported.</span></span>|
|<span data-ttu-id="0f734-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0f734-117">Application</span></span>|<span data-ttu-id="0f734-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f734-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f734-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0f734-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="0f734-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0f734-120">Request headers</span></span>
|<span data-ttu-id="0f734-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0f734-121">Header</span></span>|<span data-ttu-id="0f734-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0f734-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0f734-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0f734-123">Authorization</span></span>|<span data-ttu-id="0f734-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0f734-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0f734-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0f734-125">Accept</span></span>|<span data-ttu-id="0f734-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0f734-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f734-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0f734-127">Request body</span></span>
<span data-ttu-id="0f734-128">No corpo da solicitação, forneça uma representação JSON do objeto androidForWorkApp.</span><span class="sxs-lookup"><span data-stu-id="0f734-128">In the request body, supply a JSON representation for the androidForWorkApp object.</span></span>

<span data-ttu-id="0f734-129">A tabela a seguir mostra as propriedades que são necessárias ao criar androidForWorkApp.</span><span class="sxs-lookup"><span data-stu-id="0f734-129">The following table shows the properties that are required when you create the androidForWorkApp.</span></span>

|<span data-ttu-id="0f734-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0f734-130">Property</span></span>|<span data-ttu-id="0f734-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0f734-131">Type</span></span>|<span data-ttu-id="0f734-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f734-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f734-133">id</span><span class="sxs-lookup"><span data-stu-id="0f734-133">id</span></span>|<span data-ttu-id="0f734-134">String</span><span class="sxs-lookup"><span data-stu-id="0f734-134">String</span></span>|<span data-ttu-id="0f734-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0f734-135">Key of the entity.</span></span> <span data-ttu-id="0f734-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f734-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0f734-137">displayName</span><span class="sxs-lookup"><span data-stu-id="0f734-137">displayName</span></span>|<span data-ttu-id="0f734-138">String</span><span class="sxs-lookup"><span data-stu-id="0f734-138">String</span></span>|<span data-ttu-id="0f734-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="0f734-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="0f734-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f734-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0f734-141">description</span><span class="sxs-lookup"><span data-stu-id="0f734-141">description</span></span>|<span data-ttu-id="0f734-142">String</span><span class="sxs-lookup"><span data-stu-id="0f734-142">String</span></span>|<span data-ttu-id="0f734-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0f734-143">The description of the app.</span></span> <span data-ttu-id="0f734-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f734-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0f734-145">publicador</span><span class="sxs-lookup"><span data-stu-id="0f734-145">publisher</span></span>|<span data-ttu-id="0f734-146">String</span><span class="sxs-lookup"><span data-stu-id="0f734-146">String</span></span>|<span data-ttu-id="0f734-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0f734-147">The publisher of the app.</span></span> <span data-ttu-id="0f734-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f734-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0f734-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="0f734-149">largeIcon</span></span>|[<span data-ttu-id="0f734-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="0f734-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="0f734-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="0f734-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="0f734-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f734-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0f734-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0f734-153">createdDateTime</span></span>|<span data-ttu-id="0f734-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f734-154">DateTimeOffset</span></span>|<span data-ttu-id="0f734-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0f734-155">The date and time the app was created.</span></span> <span data-ttu-id="0f734-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f734-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0f734-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0f734-157">lastModifiedDateTime</span></span>|<span data-ttu-id="0f734-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f734-158">DateTimeOffset</span></span>|<span data-ttu-id="0f734-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="0f734-159">The date and time the app was last modified.</span></span> <span data-ttu-id="0f734-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f734-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0f734-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="0f734-161">isFeatured</span></span>|<span data-ttu-id="0f734-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f734-162">Boolean</span></span>|<span data-ttu-id="0f734-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f734-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0f734-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="0f734-164">privacyInformationUrl</span></span>|<span data-ttu-id="0f734-165">String</span><span class="sxs-lookup"><span data-stu-id="0f734-165">String</span></span>|<span data-ttu-id="0f734-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="0f734-166">The privacy statement Url.</span></span> <span data-ttu-id="0f734-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f734-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0f734-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="0f734-168">informationUrl</span></span>|<span data-ttu-id="0f734-169">String</span><span class="sxs-lookup"><span data-stu-id="0f734-169">String</span></span>|<span data-ttu-id="0f734-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="0f734-170">The more information Url.</span></span> <span data-ttu-id="0f734-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f734-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0f734-172">owner</span><span class="sxs-lookup"><span data-stu-id="0f734-172">owner</span></span>|<span data-ttu-id="0f734-173">String</span><span class="sxs-lookup"><span data-stu-id="0f734-173">String</span></span>|<span data-ttu-id="0f734-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="0f734-174">The owner of the app.</span></span> <span data-ttu-id="0f734-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f734-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0f734-176">developer</span><span class="sxs-lookup"><span data-stu-id="0f734-176">developer</span></span>|<span data-ttu-id="0f734-177">String</span><span class="sxs-lookup"><span data-stu-id="0f734-177">String</span></span>|<span data-ttu-id="0f734-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0f734-178">The developer of the app.</span></span> <span data-ttu-id="0f734-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f734-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0f734-180">notes</span><span class="sxs-lookup"><span data-stu-id="0f734-180">notes</span></span>|<span data-ttu-id="0f734-181">String</span><span class="sxs-lookup"><span data-stu-id="0f734-181">String</span></span>|<span data-ttu-id="0f734-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0f734-182">Notes for the app.</span></span> <span data-ttu-id="0f734-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f734-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0f734-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="0f734-184">uploadState</span></span>|<span data-ttu-id="0f734-185">Int32</span><span class="sxs-lookup"><span data-stu-id="0f734-185">Int32</span></span>|<span data-ttu-id="0f734-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="0f734-186">The upload state.</span></span> <span data-ttu-id="0f734-187">Os valores possíveis são: 0- `Not Ready` , 1- `Ready` , 2- `Processing` .</span><span class="sxs-lookup"><span data-stu-id="0f734-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="0f734-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f734-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0f734-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="0f734-189">publishingState</span></span>|[<span data-ttu-id="0f734-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="0f734-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="0f734-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0f734-191">The publishing state for the app.</span></span> <span data-ttu-id="0f734-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="0f734-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="0f734-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0f734-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="0f734-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="0f734-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="0f734-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="0f734-195">isAssigned</span></span>|<span data-ttu-id="0f734-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f734-196">Boolean</span></span>|<span data-ttu-id="0f734-197">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="0f734-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="0f734-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f734-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0f734-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0f734-199">roleScopeTagIds</span></span>|<span data-ttu-id="0f734-200">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f734-200">String collection</span></span>|<span data-ttu-id="0f734-201">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="0f734-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="0f734-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f734-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0f734-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="0f734-203">dependentAppCount</span></span>|<span data-ttu-id="0f734-204">Int32</span><span class="sxs-lookup"><span data-stu-id="0f734-204">Int32</span></span>|<span data-ttu-id="0f734-205">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="0f734-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="0f734-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f734-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0f734-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="0f734-207">supersedingAppCount</span></span>|<span data-ttu-id="0f734-208">Int32</span><span class="sxs-lookup"><span data-stu-id="0f734-208">Int32</span></span>|<span data-ttu-id="0f734-209">O número total de aplicativos que este aplicativo substitui direta ou indiretamente.</span><span class="sxs-lookup"><span data-stu-id="0f734-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="0f734-210">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f734-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0f734-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="0f734-211">supersededAppCount</span></span>|<span data-ttu-id="0f734-212">Int32</span><span class="sxs-lookup"><span data-stu-id="0f734-212">Int32</span></span>|<span data-ttu-id="0f734-213">O número total de aplicativos que este aplicativo está substituindo direta ou indiretamente por.</span><span class="sxs-lookup"><span data-stu-id="0f734-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="0f734-214">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f734-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0f734-215">packageId</span><span class="sxs-lookup"><span data-stu-id="0f734-215">packageId</span></span>|<span data-ttu-id="0f734-216">String</span><span class="sxs-lookup"><span data-stu-id="0f734-216">String</span></span>|<span data-ttu-id="0f734-217">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="0f734-217">The package identifier.</span></span>|
|<span data-ttu-id="0f734-218">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="0f734-218">appIdentifier</span></span>|<span data-ttu-id="0f734-219">String</span><span class="sxs-lookup"><span data-stu-id="0f734-219">String</span></span>|<span data-ttu-id="0f734-220">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="0f734-220">The Identity Name.</span></span>|
|<span data-ttu-id="0f734-221">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="0f734-221">usedLicenseCount</span></span>|<span data-ttu-id="0f734-222">Int32</span><span class="sxs-lookup"><span data-stu-id="0f734-222">Int32</span></span>|<span data-ttu-id="0f734-223">O número de aplicativos VPP em uso.</span><span class="sxs-lookup"><span data-stu-id="0f734-223">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="0f734-224">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="0f734-224">totalLicenseCount</span></span>|<span data-ttu-id="0f734-225">Int32</span><span class="sxs-lookup"><span data-stu-id="0f734-225">Int32</span></span>|<span data-ttu-id="0f734-226">O número total de licenças VPP.</span><span class="sxs-lookup"><span data-stu-id="0f734-226">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="0f734-227">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="0f734-227">appStoreUrl</span></span>|<span data-ttu-id="0f734-228">String</span><span class="sxs-lookup"><span data-stu-id="0f734-228">String</span></span>|<span data-ttu-id="0f734-229">A URL do aplicativo de reproduzir para o repositório de trabalho.</span><span class="sxs-lookup"><span data-stu-id="0f734-229">The Play for Work Store app URL.</span></span>|



## <a name="response"></a><span data-ttu-id="0f734-230">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f734-230">Response</span></span>
<span data-ttu-id="0f734-231">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0f734-231">If successful, this method returns a `201 Created` response code and a [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f734-232">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0f734-232">Example</span></span>

### <a name="request"></a><span data-ttu-id="0f734-233">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0f734-233">Request</span></span>
<span data-ttu-id="0f734-234">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0f734-234">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 960

{
  "@odata.type": "#microsoft.graph.androidForWorkApp",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```

### <a name="response"></a><span data-ttu-id="0f734-235">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f734-235">Response</span></span>
<span data-ttu-id="0f734-p121">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0f734-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1132

{
  "@odata.type": "#microsoft.graph.androidForWorkApp",
  "id": "c5010785-0785-c501-8507-01c5850701c5",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```




