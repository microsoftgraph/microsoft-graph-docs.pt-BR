---
title: Criar managedIOSStoreApp
description: Cria um novo objeto managedIOSStoreApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f594aeb3c54e0cb6abcf697034fff37a6ebfa69c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47977737"
---
# <a name="create-managediosstoreapp"></a><span data-ttu-id="a00ff-103">Criar managedIOSStoreApp</span><span class="sxs-lookup"><span data-stu-id="a00ff-103">Create managedIOSStoreApp</span></span>

<span data-ttu-id="a00ff-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a00ff-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a00ff-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a00ff-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a00ff-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a00ff-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a00ff-107">Cria um novo objeto [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="a00ff-107">Create a new [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a00ff-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a00ff-108">Prerequisites</span></span>
<span data-ttu-id="a00ff-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a00ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a00ff-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a00ff-111">Permission type</span></span>|<span data-ttu-id="a00ff-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a00ff-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a00ff-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a00ff-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a00ff-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a00ff-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a00ff-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a00ff-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a00ff-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a00ff-116">Not supported.</span></span>|
|<span data-ttu-id="a00ff-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a00ff-117">Application</span></span>|<span data-ttu-id="a00ff-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a00ff-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a00ff-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a00ff-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="a00ff-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a00ff-120">Request headers</span></span>
|<span data-ttu-id="a00ff-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a00ff-121">Header</span></span>|<span data-ttu-id="a00ff-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a00ff-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a00ff-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a00ff-123">Authorization</span></span>|<span data-ttu-id="a00ff-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a00ff-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a00ff-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a00ff-125">Accept</span></span>|<span data-ttu-id="a00ff-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a00ff-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a00ff-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a00ff-127">Request body</span></span>
<span data-ttu-id="a00ff-128">No corpo da solicitação, forneça uma representação JSON do objeto managedIOSStoreApp.</span><span class="sxs-lookup"><span data-stu-id="a00ff-128">In the request body, supply a JSON representation for the managedIOSStoreApp object.</span></span>

<span data-ttu-id="a00ff-129">A tabela a seguir mostra as propriedades obrigatórias ao criar managedIOSStoreApp.</span><span class="sxs-lookup"><span data-stu-id="a00ff-129">The following table shows the properties that are required when you create the managedIOSStoreApp.</span></span>

|<span data-ttu-id="a00ff-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a00ff-130">Property</span></span>|<span data-ttu-id="a00ff-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a00ff-131">Type</span></span>|<span data-ttu-id="a00ff-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a00ff-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a00ff-133">id</span><span class="sxs-lookup"><span data-stu-id="a00ff-133">id</span></span>|<span data-ttu-id="a00ff-134">String</span><span class="sxs-lookup"><span data-stu-id="a00ff-134">String</span></span>|<span data-ttu-id="a00ff-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a00ff-135">Key of the entity.</span></span> <span data-ttu-id="a00ff-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a00ff-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a00ff-137">displayName</span><span class="sxs-lookup"><span data-stu-id="a00ff-137">displayName</span></span>|<span data-ttu-id="a00ff-138">String</span><span class="sxs-lookup"><span data-stu-id="a00ff-138">String</span></span>|<span data-ttu-id="a00ff-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="a00ff-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="a00ff-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a00ff-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a00ff-141">description</span><span class="sxs-lookup"><span data-stu-id="a00ff-141">description</span></span>|<span data-ttu-id="a00ff-142">String</span><span class="sxs-lookup"><span data-stu-id="a00ff-142">String</span></span>|<span data-ttu-id="a00ff-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a00ff-143">The description of the app.</span></span> <span data-ttu-id="a00ff-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a00ff-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a00ff-145">publicador</span><span class="sxs-lookup"><span data-stu-id="a00ff-145">publisher</span></span>|<span data-ttu-id="a00ff-146">String</span><span class="sxs-lookup"><span data-stu-id="a00ff-146">String</span></span>|<span data-ttu-id="a00ff-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a00ff-147">The publisher of the app.</span></span> <span data-ttu-id="a00ff-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a00ff-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a00ff-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="a00ff-149">largeIcon</span></span>|[<span data-ttu-id="a00ff-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="a00ff-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="a00ff-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="a00ff-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="a00ff-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a00ff-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a00ff-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a00ff-153">createdDateTime</span></span>|<span data-ttu-id="a00ff-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a00ff-154">DateTimeOffset</span></span>|<span data-ttu-id="a00ff-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a00ff-155">The date and time the app was created.</span></span> <span data-ttu-id="a00ff-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a00ff-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a00ff-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a00ff-157">lastModifiedDateTime</span></span>|<span data-ttu-id="a00ff-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a00ff-158">DateTimeOffset</span></span>|<span data-ttu-id="a00ff-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="a00ff-159">The date and time the app was last modified.</span></span> <span data-ttu-id="a00ff-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a00ff-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a00ff-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="a00ff-161">isFeatured</span></span>|<span data-ttu-id="a00ff-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="a00ff-162">Boolean</span></span>|<span data-ttu-id="a00ff-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a00ff-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a00ff-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="a00ff-164">privacyInformationUrl</span></span>|<span data-ttu-id="a00ff-165">String</span><span class="sxs-lookup"><span data-stu-id="a00ff-165">String</span></span>|<span data-ttu-id="a00ff-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="a00ff-166">The privacy statement Url.</span></span> <span data-ttu-id="a00ff-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a00ff-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a00ff-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="a00ff-168">informationUrl</span></span>|<span data-ttu-id="a00ff-169">String</span><span class="sxs-lookup"><span data-stu-id="a00ff-169">String</span></span>|<span data-ttu-id="a00ff-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="a00ff-170">The more information Url.</span></span> <span data-ttu-id="a00ff-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a00ff-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a00ff-172">proprietário</span><span class="sxs-lookup"><span data-stu-id="a00ff-172">owner</span></span>|<span data-ttu-id="a00ff-173">String</span><span class="sxs-lookup"><span data-stu-id="a00ff-173">String</span></span>|<span data-ttu-id="a00ff-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="a00ff-174">The owner of the app.</span></span> <span data-ttu-id="a00ff-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a00ff-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a00ff-176">developer</span><span class="sxs-lookup"><span data-stu-id="a00ff-176">developer</span></span>|<span data-ttu-id="a00ff-177">String</span><span class="sxs-lookup"><span data-stu-id="a00ff-177">String</span></span>|<span data-ttu-id="a00ff-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a00ff-178">The developer of the app.</span></span> <span data-ttu-id="a00ff-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a00ff-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a00ff-180">notes</span><span class="sxs-lookup"><span data-stu-id="a00ff-180">notes</span></span>|<span data-ttu-id="a00ff-181">String</span><span class="sxs-lookup"><span data-stu-id="a00ff-181">String</span></span>|<span data-ttu-id="a00ff-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a00ff-182">Notes for the app.</span></span> <span data-ttu-id="a00ff-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a00ff-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a00ff-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="a00ff-184">uploadState</span></span>|<span data-ttu-id="a00ff-185">Int32</span><span class="sxs-lookup"><span data-stu-id="a00ff-185">Int32</span></span>|<span data-ttu-id="a00ff-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="a00ff-186">The upload state.</span></span> <span data-ttu-id="a00ff-187">Os valores possíveis são: 0- `Not Ready` , 1- `Ready` , 2- `Processing` .</span><span class="sxs-lookup"><span data-stu-id="a00ff-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="a00ff-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a00ff-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a00ff-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="a00ff-189">publishingState</span></span>|[<span data-ttu-id="a00ff-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="a00ff-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="a00ff-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a00ff-191">The publishing state for the app.</span></span> <span data-ttu-id="a00ff-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="a00ff-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="a00ff-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a00ff-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="a00ff-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="a00ff-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="a00ff-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="a00ff-195">isAssigned</span></span>|<span data-ttu-id="a00ff-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="a00ff-196">Boolean</span></span>|<span data-ttu-id="a00ff-197">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="a00ff-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="a00ff-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a00ff-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a00ff-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a00ff-199">roleScopeTagIds</span></span>|<span data-ttu-id="a00ff-200">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a00ff-200">String collection</span></span>|<span data-ttu-id="a00ff-201">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="a00ff-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="a00ff-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a00ff-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a00ff-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="a00ff-203">dependentAppCount</span></span>|<span data-ttu-id="a00ff-204">Int32</span><span class="sxs-lookup"><span data-stu-id="a00ff-204">Int32</span></span>|<span data-ttu-id="a00ff-205">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="a00ff-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="a00ff-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a00ff-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a00ff-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="a00ff-207">supersedingAppCount</span></span>|<span data-ttu-id="a00ff-208">Int32</span><span class="sxs-lookup"><span data-stu-id="a00ff-208">Int32</span></span>|<span data-ttu-id="a00ff-209">O número total de aplicativos que este aplicativo substitui direta ou indiretamente.</span><span class="sxs-lookup"><span data-stu-id="a00ff-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="a00ff-210">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a00ff-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a00ff-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="a00ff-211">supersededAppCount</span></span>|<span data-ttu-id="a00ff-212">Int32</span><span class="sxs-lookup"><span data-stu-id="a00ff-212">Int32</span></span>|<span data-ttu-id="a00ff-213">O número total de aplicativos que este aplicativo está substituindo direta ou indiretamente por.</span><span class="sxs-lookup"><span data-stu-id="a00ff-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="a00ff-214">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a00ff-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a00ff-215">appAvailability</span><span class="sxs-lookup"><span data-stu-id="a00ff-215">appAvailability</span></span>|[<span data-ttu-id="a00ff-216">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="a00ff-216">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="a00ff-217">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a00ff-217">The Application's availability.</span></span> <span data-ttu-id="a00ff-218">Herdado de [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="a00ff-218">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="a00ff-219">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="a00ff-219">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="a00ff-220">version</span><span class="sxs-lookup"><span data-stu-id="a00ff-220">version</span></span>|<span data-ttu-id="a00ff-221">String</span><span class="sxs-lookup"><span data-stu-id="a00ff-221">String</span></span>|<span data-ttu-id="a00ff-222">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a00ff-222">The Application's version.</span></span> <span data-ttu-id="a00ff-223">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="a00ff-223">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="a00ff-224">bundleId</span><span class="sxs-lookup"><span data-stu-id="a00ff-224">bundleId</span></span>|<span data-ttu-id="a00ff-225">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a00ff-225">String</span></span>|<span data-ttu-id="a00ff-226">A ID do pacote de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="a00ff-226">The app's Bundle ID.</span></span>|
|<span data-ttu-id="a00ff-227">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="a00ff-227">appStoreUrl</span></span>|<span data-ttu-id="a00ff-228">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a00ff-228">String</span></span>|<span data-ttu-id="a00ff-229">A AppStoreUrl da Apple.</span><span class="sxs-lookup"><span data-stu-id="a00ff-229">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="a00ff-230">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="a00ff-230">applicableDeviceType</span></span>|[<span data-ttu-id="a00ff-231">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="a00ff-231">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="a00ff-232">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="a00ff-232">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="a00ff-233">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="a00ff-233">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="a00ff-234">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="a00ff-234">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="a00ff-235">O valor do sistema operacional mínimo com suporte.</span><span class="sxs-lookup"><span data-stu-id="a00ff-235">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="a00ff-236">Resposta</span><span class="sxs-lookup"><span data-stu-id="a00ff-236">Response</span></span>
<span data-ttu-id="a00ff-237">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a00ff-237">If successful, this method returns a `201 Created` response code and a [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a00ff-238">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a00ff-238">Example</span></span>

### <a name="request"></a><span data-ttu-id="a00ff-239">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a00ff-239">Request</span></span>
<span data-ttu-id="a00ff-240">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a00ff-240">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1295

{
  "@odata.type": "#microsoft.graph.managedIOSStoreApp",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true,
    "v13_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="a00ff-241">Resposta</span><span class="sxs-lookup"><span data-stu-id="a00ff-241">Response</span></span>
<span data-ttu-id="a00ff-p123">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a00ff-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1467

{
  "@odata.type": "#microsoft.graph.managedIOSStoreApp",
  "id": "51b9830f-830f-51b9-0f83-b9510f83b951",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true,
    "v13_0": true
  }
}
```






