---
title: Atualizar managedIOSStoreApp
description: Atualiza as propriedades de um objeto managedIOSStoreApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e25edd1a71ae8d53084a661f385f54285b8fc86b
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48699202"
---
# <a name="update-managediosstoreapp"></a><span data-ttu-id="78619-103">Atualizar managedIOSStoreApp</span><span class="sxs-lookup"><span data-stu-id="78619-103">Update managedIOSStoreApp</span></span>

<span data-ttu-id="78619-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78619-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="78619-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="78619-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="78619-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="78619-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="78619-107">Atualiza as propriedades de um objeto [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="78619-107">Update the properties of a [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="78619-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="78619-108">Prerequisites</span></span>
<span data-ttu-id="78619-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78619-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78619-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="78619-111">Permission type</span></span>|<span data-ttu-id="78619-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="78619-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="78619-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="78619-113">Delegated (work or school account)</span></span>|<span data-ttu-id="78619-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78619-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="78619-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="78619-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="78619-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="78619-116">Not supported.</span></span>|
|<span data-ttu-id="78619-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="78619-117">Application</span></span>|<span data-ttu-id="78619-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78619-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="78619-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="78619-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="78619-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="78619-120">Request headers</span></span>
|<span data-ttu-id="78619-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="78619-121">Header</span></span>|<span data-ttu-id="78619-122">Valor</span><span class="sxs-lookup"><span data-stu-id="78619-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="78619-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="78619-123">Authorization</span></span>|<span data-ttu-id="78619-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="78619-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="78619-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="78619-125">Accept</span></span>|<span data-ttu-id="78619-126">application/json</span><span class="sxs-lookup"><span data-stu-id="78619-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="78619-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="78619-127">Request body</span></span>
<span data-ttu-id="78619-128">No corpo da solicitação, forneça uma representação JSON do objeto [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="78619-128">In the request body, supply a JSON representation for the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

<span data-ttu-id="78619-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="78619-129">The following table shows the properties that are required when you create the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span></span>

|<span data-ttu-id="78619-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="78619-130">Property</span></span>|<span data-ttu-id="78619-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="78619-131">Type</span></span>|<span data-ttu-id="78619-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="78619-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78619-133">id</span><span class="sxs-lookup"><span data-stu-id="78619-133">id</span></span>|<span data-ttu-id="78619-134">String</span><span class="sxs-lookup"><span data-stu-id="78619-134">String</span></span>|<span data-ttu-id="78619-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="78619-135">Key of the entity.</span></span> <span data-ttu-id="78619-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="78619-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="78619-137">displayName</span><span class="sxs-lookup"><span data-stu-id="78619-137">displayName</span></span>|<span data-ttu-id="78619-138">String</span><span class="sxs-lookup"><span data-stu-id="78619-138">String</span></span>|<span data-ttu-id="78619-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="78619-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="78619-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="78619-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="78619-141">description</span><span class="sxs-lookup"><span data-stu-id="78619-141">description</span></span>|<span data-ttu-id="78619-142">String</span><span class="sxs-lookup"><span data-stu-id="78619-142">String</span></span>|<span data-ttu-id="78619-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="78619-143">The description of the app.</span></span> <span data-ttu-id="78619-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="78619-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="78619-145">publicador</span><span class="sxs-lookup"><span data-stu-id="78619-145">publisher</span></span>|<span data-ttu-id="78619-146">String</span><span class="sxs-lookup"><span data-stu-id="78619-146">String</span></span>|<span data-ttu-id="78619-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="78619-147">The publisher of the app.</span></span> <span data-ttu-id="78619-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="78619-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="78619-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="78619-149">largeIcon</span></span>|[<span data-ttu-id="78619-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="78619-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="78619-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="78619-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="78619-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="78619-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="78619-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="78619-153">createdDateTime</span></span>|<span data-ttu-id="78619-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78619-154">DateTimeOffset</span></span>|<span data-ttu-id="78619-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="78619-155">The date and time the app was created.</span></span> <span data-ttu-id="78619-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="78619-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="78619-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="78619-157">lastModifiedDateTime</span></span>|<span data-ttu-id="78619-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78619-158">DateTimeOffset</span></span>|<span data-ttu-id="78619-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="78619-159">The date and time the app was last modified.</span></span> <span data-ttu-id="78619-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="78619-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="78619-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="78619-161">isFeatured</span></span>|<span data-ttu-id="78619-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="78619-162">Boolean</span></span>|<span data-ttu-id="78619-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="78619-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="78619-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="78619-164">privacyInformationUrl</span></span>|<span data-ttu-id="78619-165">String</span><span class="sxs-lookup"><span data-stu-id="78619-165">String</span></span>|<span data-ttu-id="78619-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="78619-166">The privacy statement Url.</span></span> <span data-ttu-id="78619-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="78619-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="78619-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="78619-168">informationUrl</span></span>|<span data-ttu-id="78619-169">String</span><span class="sxs-lookup"><span data-stu-id="78619-169">String</span></span>|<span data-ttu-id="78619-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="78619-170">The more information Url.</span></span> <span data-ttu-id="78619-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="78619-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="78619-172">owner</span><span class="sxs-lookup"><span data-stu-id="78619-172">owner</span></span>|<span data-ttu-id="78619-173">String</span><span class="sxs-lookup"><span data-stu-id="78619-173">String</span></span>|<span data-ttu-id="78619-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="78619-174">The owner of the app.</span></span> <span data-ttu-id="78619-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="78619-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="78619-176">developer</span><span class="sxs-lookup"><span data-stu-id="78619-176">developer</span></span>|<span data-ttu-id="78619-177">String</span><span class="sxs-lookup"><span data-stu-id="78619-177">String</span></span>|<span data-ttu-id="78619-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="78619-178">The developer of the app.</span></span> <span data-ttu-id="78619-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="78619-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="78619-180">notes</span><span class="sxs-lookup"><span data-stu-id="78619-180">notes</span></span>|<span data-ttu-id="78619-181">String</span><span class="sxs-lookup"><span data-stu-id="78619-181">String</span></span>|<span data-ttu-id="78619-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="78619-182">Notes for the app.</span></span> <span data-ttu-id="78619-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="78619-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="78619-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="78619-184">uploadState</span></span>|<span data-ttu-id="78619-185">Int32</span><span class="sxs-lookup"><span data-stu-id="78619-185">Int32</span></span>|<span data-ttu-id="78619-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="78619-186">The upload state.</span></span> <span data-ttu-id="78619-187">Os valores possíveis são: 0- `Not Ready` , 1- `Ready` , 2- `Processing` .</span><span class="sxs-lookup"><span data-stu-id="78619-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="78619-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="78619-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="78619-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="78619-189">publishingState</span></span>|[<span data-ttu-id="78619-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="78619-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="78619-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="78619-191">The publishing state for the app.</span></span> <span data-ttu-id="78619-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="78619-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="78619-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="78619-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="78619-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="78619-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="78619-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="78619-195">isAssigned</span></span>|<span data-ttu-id="78619-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="78619-196">Boolean</span></span>|<span data-ttu-id="78619-197">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="78619-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="78619-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="78619-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="78619-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="78619-199">roleScopeTagIds</span></span>|<span data-ttu-id="78619-200">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="78619-200">String collection</span></span>|<span data-ttu-id="78619-201">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="78619-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="78619-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="78619-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="78619-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="78619-203">dependentAppCount</span></span>|<span data-ttu-id="78619-204">Int32</span><span class="sxs-lookup"><span data-stu-id="78619-204">Int32</span></span>|<span data-ttu-id="78619-205">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="78619-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="78619-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="78619-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="78619-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="78619-207">supersedingAppCount</span></span>|<span data-ttu-id="78619-208">Int32</span><span class="sxs-lookup"><span data-stu-id="78619-208">Int32</span></span>|<span data-ttu-id="78619-209">O número total de aplicativos que este aplicativo substitui direta ou indiretamente.</span><span class="sxs-lookup"><span data-stu-id="78619-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="78619-210">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="78619-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="78619-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="78619-211">supersededAppCount</span></span>|<span data-ttu-id="78619-212">Int32</span><span class="sxs-lookup"><span data-stu-id="78619-212">Int32</span></span>|<span data-ttu-id="78619-213">O número total de aplicativos que este aplicativo está substituindo direta ou indiretamente por.</span><span class="sxs-lookup"><span data-stu-id="78619-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="78619-214">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="78619-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="78619-215">appAvailability</span><span class="sxs-lookup"><span data-stu-id="78619-215">appAvailability</span></span>|[<span data-ttu-id="78619-216">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="78619-216">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="78619-217">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="78619-217">The Application's availability.</span></span> <span data-ttu-id="78619-218">Herdado de [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="78619-218">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="78619-219">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="78619-219">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="78619-220">version</span><span class="sxs-lookup"><span data-stu-id="78619-220">version</span></span>|<span data-ttu-id="78619-221">String</span><span class="sxs-lookup"><span data-stu-id="78619-221">String</span></span>|<span data-ttu-id="78619-222">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="78619-222">The Application's version.</span></span> <span data-ttu-id="78619-223">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="78619-223">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="78619-224">bundleId</span><span class="sxs-lookup"><span data-stu-id="78619-224">bundleId</span></span>|<span data-ttu-id="78619-225">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="78619-225">String</span></span>|<span data-ttu-id="78619-226">A ID do pacote de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="78619-226">The app's Bundle ID.</span></span>|
|<span data-ttu-id="78619-227">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="78619-227">appStoreUrl</span></span>|<span data-ttu-id="78619-228">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="78619-228">String</span></span>|<span data-ttu-id="78619-229">A AppStoreUrl da Apple.</span><span class="sxs-lookup"><span data-stu-id="78619-229">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="78619-230">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="78619-230">applicableDeviceType</span></span>|[<span data-ttu-id="78619-231">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="78619-231">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="78619-232">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="78619-232">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="78619-233">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="78619-233">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="78619-234">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="78619-234">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="78619-235">O valor do sistema operacional mínimo com suporte.</span><span class="sxs-lookup"><span data-stu-id="78619-235">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="78619-236">Resposta</span><span class="sxs-lookup"><span data-stu-id="78619-236">Response</span></span>
<span data-ttu-id="78619-237">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="78619-237">If successful, this method returns a `200 OK` response code and an updated [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78619-238">Exemplo</span><span class="sxs-lookup"><span data-stu-id="78619-238">Example</span></span>

### <a name="request"></a><span data-ttu-id="78619-239">Solicitação</span><span class="sxs-lookup"><span data-stu-id="78619-239">Request</span></span>
<span data-ttu-id="78619-240">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="78619-240">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
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

### <a name="response"></a><span data-ttu-id="78619-241">Resposta</span><span class="sxs-lookup"><span data-stu-id="78619-241">Response</span></span>
<span data-ttu-id="78619-p123">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="78619-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





