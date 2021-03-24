---
title: Atualizar managedIOSStoreApp
description: Atualiza as propriedades de um objeto managedIOSStoreApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8943f032f55fc19831d2828d22aea332f049c8e8
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51140011"
---
# <a name="update-managediosstoreapp"></a><span data-ttu-id="f3135-103">Atualizar managedIOSStoreApp</span><span class="sxs-lookup"><span data-stu-id="f3135-103">Update managedIOSStoreApp</span></span>

<span data-ttu-id="f3135-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3135-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f3135-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f3135-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3135-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f3135-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3135-107">Atualiza as propriedades de um objeto [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3135-107">Update the properties of a [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f3135-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f3135-108">Prerequisites</span></span>
<span data-ttu-id="f3135-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3135-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3135-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f3135-111">Permission type</span></span>|<span data-ttu-id="f3135-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f3135-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3135-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f3135-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f3135-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3135-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f3135-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f3135-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3135-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f3135-116">Not supported.</span></span>|
|<span data-ttu-id="f3135-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f3135-117">Application</span></span>|<span data-ttu-id="f3135-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3135-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3135-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f3135-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="f3135-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f3135-120">Request headers</span></span>
|<span data-ttu-id="f3135-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f3135-121">Header</span></span>|<span data-ttu-id="f3135-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f3135-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3135-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f3135-123">Authorization</span></span>|<span data-ttu-id="f3135-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f3135-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3135-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f3135-125">Accept</span></span>|<span data-ttu-id="f3135-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f3135-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3135-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f3135-127">Request body</span></span>
<span data-ttu-id="f3135-128">No corpo da solicitação, forneça uma representação JSON do objeto [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3135-128">In the request body, supply a JSON representation for the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

<span data-ttu-id="f3135-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3135-129">The following table shows the properties that are required when you create the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span></span>

|<span data-ttu-id="f3135-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f3135-130">Property</span></span>|<span data-ttu-id="f3135-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f3135-131">Type</span></span>|<span data-ttu-id="f3135-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3135-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3135-133">id</span><span class="sxs-lookup"><span data-stu-id="f3135-133">id</span></span>|<span data-ttu-id="f3135-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f3135-134">String</span></span>|<span data-ttu-id="f3135-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f3135-135">Key of the entity.</span></span> <span data-ttu-id="f3135-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f3135-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f3135-137">displayName</span><span class="sxs-lookup"><span data-stu-id="f3135-137">displayName</span></span>|<span data-ttu-id="f3135-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f3135-138">String</span></span>|<span data-ttu-id="f3135-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="f3135-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="f3135-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f3135-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f3135-141">descrição</span><span class="sxs-lookup"><span data-stu-id="f3135-141">description</span></span>|<span data-ttu-id="f3135-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f3135-142">String</span></span>|<span data-ttu-id="f3135-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f3135-143">The description of the app.</span></span> <span data-ttu-id="f3135-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f3135-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f3135-145">publicador</span><span class="sxs-lookup"><span data-stu-id="f3135-145">publisher</span></span>|<span data-ttu-id="f3135-146">String</span><span class="sxs-lookup"><span data-stu-id="f3135-146">String</span></span>|<span data-ttu-id="f3135-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f3135-147">The publisher of the app.</span></span> <span data-ttu-id="f3135-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f3135-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f3135-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="f3135-149">largeIcon</span></span>|[<span data-ttu-id="f3135-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f3135-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f3135-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="f3135-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="f3135-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f3135-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f3135-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f3135-153">createdDateTime</span></span>|<span data-ttu-id="f3135-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3135-154">DateTimeOffset</span></span>|<span data-ttu-id="f3135-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f3135-155">The date and time the app was created.</span></span> <span data-ttu-id="f3135-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f3135-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f3135-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f3135-157">lastModifiedDateTime</span></span>|<span data-ttu-id="f3135-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3135-158">DateTimeOffset</span></span>|<span data-ttu-id="f3135-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="f3135-159">The date and time the app was last modified.</span></span> <span data-ttu-id="f3135-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f3135-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f3135-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="f3135-161">isFeatured</span></span>|<span data-ttu-id="f3135-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3135-162">Boolean</span></span>|<span data-ttu-id="f3135-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f3135-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f3135-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f3135-164">privacyInformationUrl</span></span>|<span data-ttu-id="f3135-165">String</span><span class="sxs-lookup"><span data-stu-id="f3135-165">String</span></span>|<span data-ttu-id="f3135-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="f3135-166">The privacy statement Url.</span></span> <span data-ttu-id="f3135-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f3135-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f3135-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f3135-168">informationUrl</span></span>|<span data-ttu-id="f3135-169">String</span><span class="sxs-lookup"><span data-stu-id="f3135-169">String</span></span>|<span data-ttu-id="f3135-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="f3135-170">The more information Url.</span></span> <span data-ttu-id="f3135-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f3135-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f3135-172">owner</span><span class="sxs-lookup"><span data-stu-id="f3135-172">owner</span></span>|<span data-ttu-id="f3135-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f3135-173">String</span></span>|<span data-ttu-id="f3135-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="f3135-174">The owner of the app.</span></span> <span data-ttu-id="f3135-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f3135-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f3135-176">developer</span><span class="sxs-lookup"><span data-stu-id="f3135-176">developer</span></span>|<span data-ttu-id="f3135-177">String</span><span class="sxs-lookup"><span data-stu-id="f3135-177">String</span></span>|<span data-ttu-id="f3135-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f3135-178">The developer of the app.</span></span> <span data-ttu-id="f3135-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f3135-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f3135-180">notes</span><span class="sxs-lookup"><span data-stu-id="f3135-180">notes</span></span>|<span data-ttu-id="f3135-181">String</span><span class="sxs-lookup"><span data-stu-id="f3135-181">String</span></span>|<span data-ttu-id="f3135-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f3135-182">Notes for the app.</span></span> <span data-ttu-id="f3135-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f3135-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f3135-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="f3135-184">uploadState</span></span>|<span data-ttu-id="f3135-185">Int32</span><span class="sxs-lookup"><span data-stu-id="f3135-185">Int32</span></span>|<span data-ttu-id="f3135-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="f3135-186">The upload state.</span></span> <span data-ttu-id="f3135-187">Os valores possíveis são: 0 - `Not Ready` , 1 - `Ready` , 2 - `Processing` .</span><span class="sxs-lookup"><span data-stu-id="f3135-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="f3135-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f3135-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f3135-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="f3135-189">publishingState</span></span>|[<span data-ttu-id="f3135-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="f3135-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="f3135-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f3135-191">The publishing state for the app.</span></span> <span data-ttu-id="f3135-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="f3135-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="f3135-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3135-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="f3135-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="f3135-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="f3135-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="f3135-195">isAssigned</span></span>|<span data-ttu-id="f3135-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3135-196">Boolean</span></span>|<span data-ttu-id="f3135-197">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="f3135-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="f3135-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f3135-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f3135-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f3135-199">roleScopeTagIds</span></span>|<span data-ttu-id="f3135-200">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f3135-200">String collection</span></span>|<span data-ttu-id="f3135-201">Lista de ids de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="f3135-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="f3135-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f3135-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f3135-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="f3135-203">dependentAppCount</span></span>|<span data-ttu-id="f3135-204">Int32</span><span class="sxs-lookup"><span data-stu-id="f3135-204">Int32</span></span>|<span data-ttu-id="f3135-205">O número total de dependências que o aplicativo filho tem.</span><span class="sxs-lookup"><span data-stu-id="f3135-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="f3135-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f3135-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f3135-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="f3135-207">supersedingAppCount</span></span>|<span data-ttu-id="f3135-208">Int32</span><span class="sxs-lookup"><span data-stu-id="f3135-208">Int32</span></span>|<span data-ttu-id="f3135-209">O número total de aplicativos que esse aplicativo sobressede direta ou indiretamente.</span><span class="sxs-lookup"><span data-stu-id="f3135-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="f3135-210">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f3135-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f3135-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="f3135-211">supersededAppCount</span></span>|<span data-ttu-id="f3135-212">Int32</span><span class="sxs-lookup"><span data-stu-id="f3135-212">Int32</span></span>|<span data-ttu-id="f3135-213">O número total de aplicativos pelos quais esse aplicativo é, direta ou indiretamente, é suplido.</span><span class="sxs-lookup"><span data-stu-id="f3135-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="f3135-214">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f3135-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f3135-215">appAvailability</span><span class="sxs-lookup"><span data-stu-id="f3135-215">appAvailability</span></span>|[<span data-ttu-id="f3135-216">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="f3135-216">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="f3135-217">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f3135-217">The Application's availability.</span></span> <span data-ttu-id="f3135-218">Herdado [de managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="f3135-218">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="f3135-219">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="f3135-219">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="f3135-220">version</span><span class="sxs-lookup"><span data-stu-id="f3135-220">version</span></span>|<span data-ttu-id="f3135-221">String</span><span class="sxs-lookup"><span data-stu-id="f3135-221">String</span></span>|<span data-ttu-id="f3135-222">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f3135-222">The Application's version.</span></span> <span data-ttu-id="f3135-223">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="f3135-223">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="f3135-224">bundleId</span><span class="sxs-lookup"><span data-stu-id="f3135-224">bundleId</span></span>|<span data-ttu-id="f3135-225">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f3135-225">String</span></span>|<span data-ttu-id="f3135-226">A ID do pacote de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="f3135-226">The app's Bundle ID.</span></span>|
|<span data-ttu-id="f3135-227">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="f3135-227">appStoreUrl</span></span>|<span data-ttu-id="f3135-228">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f3135-228">String</span></span>|<span data-ttu-id="f3135-229">A AppStoreUrl da Apple.</span><span class="sxs-lookup"><span data-stu-id="f3135-229">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="f3135-230">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="f3135-230">applicableDeviceType</span></span>|[<span data-ttu-id="f3135-231">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="f3135-231">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="f3135-232">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="f3135-232">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="f3135-233">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f3135-233">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="f3135-234">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f3135-234">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="f3135-235">O valor do sistema operacional mínimo com suporte.</span><span class="sxs-lookup"><span data-stu-id="f3135-235">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="f3135-236">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3135-236">Response</span></span>
<span data-ttu-id="f3135-237">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f3135-237">If successful, this method returns a `200 OK` response code and an updated [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3135-238">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f3135-238">Example</span></span>

### <a name="request"></a><span data-ttu-id="f3135-239">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f3135-239">Request</span></span>
<span data-ttu-id="f3135-240">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f3135-240">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1315

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
    "v13_0": true,
    "v14_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="f3135-241">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3135-241">Response</span></span>
<span data-ttu-id="f3135-p123">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f3135-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1487

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
    "v13_0": true,
    "v14_0": true
  }
}
```




