---
title: Atualizar managedIOSLobApp
description: Atualiza as propriedades de um objeto managedIOSLobApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6daab4d3395be1fc61d77e421650e8bfa07491c1
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39936623"
---
# <a name="update-managedioslobapp"></a><span data-ttu-id="2d3d9-103">Atualizar managedIOSLobApp</span><span class="sxs-lookup"><span data-stu-id="2d3d9-103">Update managedIOSLobApp</span></span>

> <span data-ttu-id="2d3d9-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2d3d9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2d3d9-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2d3d9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d3d9-106">Atualiza as propriedades de um objeto [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="2d3d9-106">Update the properties of a [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2d3d9-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2d3d9-107">Prerequisites</span></span>
<span data-ttu-id="2d3d9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d3d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d3d9-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2d3d9-110">Permission type</span></span>|<span data-ttu-id="2d3d9-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2d3d9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2d3d9-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2d3d9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2d3d9-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d3d9-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2d3d9-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2d3d9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2d3d9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2d3d9-115">Not supported.</span></span>|
|<span data-ttu-id="2d3d9-116">Application</span><span class="sxs-lookup"><span data-stu-id="2d3d9-116">Application</span></span>|<span data-ttu-id="2d3d9-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d3d9-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2d3d9-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2d3d9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="2d3d9-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2d3d9-119">Request headers</span></span>
|<span data-ttu-id="2d3d9-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2d3d9-120">Header</span></span>|<span data-ttu-id="2d3d9-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2d3d9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2d3d9-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2d3d9-122">Authorization</span></span>|<span data-ttu-id="2d3d9-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2d3d9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2d3d9-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2d3d9-124">Accept</span></span>|<span data-ttu-id="2d3d9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2d3d9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d3d9-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2d3d9-126">Request body</span></span>
<span data-ttu-id="2d3d9-127">No corpo da solicitação, forneça uma representação JSON do objeto [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="2d3d9-127">In the request body, supply a JSON representation for the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

<span data-ttu-id="2d3d9-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="2d3d9-128">The following table shows the properties that are required when you create the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span></span>

|<span data-ttu-id="2d3d9-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2d3d9-129">Property</span></span>|<span data-ttu-id="2d3d9-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="2d3d9-130">Type</span></span>|<span data-ttu-id="2d3d9-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d3d9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d3d9-132">id</span><span class="sxs-lookup"><span data-stu-id="2d3d9-132">id</span></span>|<span data-ttu-id="2d3d9-133">String</span><span class="sxs-lookup"><span data-stu-id="2d3d9-133">String</span></span>|<span data-ttu-id="2d3d9-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2d3d9-134">Key of the entity.</span></span> <span data-ttu-id="2d3d9-135">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2d3d9-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2d3d9-136">displayName</span><span class="sxs-lookup"><span data-stu-id="2d3d9-136">displayName</span></span>|<span data-ttu-id="2d3d9-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2d3d9-137">String</span></span>|<span data-ttu-id="2d3d9-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="2d3d9-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="2d3d9-139">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2d3d9-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2d3d9-140">description</span><span class="sxs-lookup"><span data-stu-id="2d3d9-140">description</span></span>|<span data-ttu-id="2d3d9-141">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="2d3d9-141">String</span></span>|<span data-ttu-id="2d3d9-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2d3d9-142">The description of the app.</span></span> <span data-ttu-id="2d3d9-143">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2d3d9-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2d3d9-144">publicador</span><span class="sxs-lookup"><span data-stu-id="2d3d9-144">publisher</span></span>|<span data-ttu-id="2d3d9-145">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="2d3d9-145">String</span></span>|<span data-ttu-id="2d3d9-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2d3d9-146">The publisher of the app.</span></span> <span data-ttu-id="2d3d9-147">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2d3d9-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2d3d9-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="2d3d9-148">largeIcon</span></span>|[<span data-ttu-id="2d3d9-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="2d3d9-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="2d3d9-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="2d3d9-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="2d3d9-151">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2d3d9-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2d3d9-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2d3d9-152">createdDateTime</span></span>|<span data-ttu-id="2d3d9-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d3d9-153">DateTimeOffset</span></span>|<span data-ttu-id="2d3d9-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2d3d9-154">The date and time the app was created.</span></span> <span data-ttu-id="2d3d9-155">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2d3d9-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2d3d9-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2d3d9-156">lastModifiedDateTime</span></span>|<span data-ttu-id="2d3d9-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d3d9-157">DateTimeOffset</span></span>|<span data-ttu-id="2d3d9-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="2d3d9-158">The date and time the app was last modified.</span></span> <span data-ttu-id="2d3d9-159">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2d3d9-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2d3d9-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="2d3d9-160">isFeatured</span></span>|<span data-ttu-id="2d3d9-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="2d3d9-161">Boolean</span></span>|<span data-ttu-id="2d3d9-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2d3d9-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2d3d9-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="2d3d9-163">privacyInformationUrl</span></span>|<span data-ttu-id="2d3d9-164">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="2d3d9-164">String</span></span>|<span data-ttu-id="2d3d9-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="2d3d9-165">The privacy statement Url.</span></span> <span data-ttu-id="2d3d9-166">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2d3d9-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2d3d9-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="2d3d9-167">informationUrl</span></span>|<span data-ttu-id="2d3d9-168">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="2d3d9-168">String</span></span>|<span data-ttu-id="2d3d9-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="2d3d9-169">The more information Url.</span></span> <span data-ttu-id="2d3d9-170">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2d3d9-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2d3d9-171">owner</span><span class="sxs-lookup"><span data-stu-id="2d3d9-171">owner</span></span>|<span data-ttu-id="2d3d9-172">String</span><span class="sxs-lookup"><span data-stu-id="2d3d9-172">String</span></span>|<span data-ttu-id="2d3d9-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="2d3d9-173">The owner of the app.</span></span> <span data-ttu-id="2d3d9-174">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2d3d9-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2d3d9-175">developer</span><span class="sxs-lookup"><span data-stu-id="2d3d9-175">developer</span></span>|<span data-ttu-id="2d3d9-176">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="2d3d9-176">String</span></span>|<span data-ttu-id="2d3d9-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2d3d9-177">The developer of the app.</span></span> <span data-ttu-id="2d3d9-178">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2d3d9-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2d3d9-179">notes</span><span class="sxs-lookup"><span data-stu-id="2d3d9-179">notes</span></span>|<span data-ttu-id="2d3d9-180">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="2d3d9-180">String</span></span>|<span data-ttu-id="2d3d9-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2d3d9-181">Notes for the app.</span></span> <span data-ttu-id="2d3d9-182">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2d3d9-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2d3d9-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="2d3d9-183">uploadState</span></span>|<span data-ttu-id="2d3d9-184">Int32</span><span class="sxs-lookup"><span data-stu-id="2d3d9-184">Int32</span></span>|<span data-ttu-id="2d3d9-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="2d3d9-185">The upload state.</span></span> <span data-ttu-id="2d3d9-186">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2d3d9-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2d3d9-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="2d3d9-187">publishingState</span></span>|[<span data-ttu-id="2d3d9-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="2d3d9-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="2d3d9-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2d3d9-189">The publishing state for the app.</span></span> <span data-ttu-id="2d3d9-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="2d3d9-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="2d3d9-191">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2d3d9-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="2d3d9-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="2d3d9-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="2d3d9-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="2d3d9-193">isAssigned</span></span>|<span data-ttu-id="2d3d9-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="2d3d9-194">Boolean</span></span>|<span data-ttu-id="2d3d9-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="2d3d9-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="2d3d9-196">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2d3d9-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2d3d9-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2d3d9-197">roleScopeTagIds</span></span>|<span data-ttu-id="2d3d9-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="2d3d9-198">String collection</span></span>|<span data-ttu-id="2d3d9-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="2d3d9-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="2d3d9-200">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2d3d9-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2d3d9-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="2d3d9-201">dependentAppCount</span></span>|<span data-ttu-id="2d3d9-202">Int32</span><span class="sxs-lookup"><span data-stu-id="2d3d9-202">Int32</span></span>|<span data-ttu-id="2d3d9-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="2d3d9-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="2d3d9-204">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2d3d9-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2d3d9-205">appAvailability</span><span class="sxs-lookup"><span data-stu-id="2d3d9-205">appAvailability</span></span>|[<span data-ttu-id="2d3d9-206">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="2d3d9-206">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="2d3d9-207">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2d3d9-207">The Application's availability.</span></span> <span data-ttu-id="2d3d9-208">Herdado de [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="2d3d9-208">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="2d3d9-209">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="2d3d9-209">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="2d3d9-210">version</span><span class="sxs-lookup"><span data-stu-id="2d3d9-210">version</span></span>|<span data-ttu-id="2d3d9-211">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2d3d9-211">String</span></span>|<span data-ttu-id="2d3d9-212">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2d3d9-212">The Application's version.</span></span> <span data-ttu-id="2d3d9-213">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="2d3d9-213">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="2d3d9-214">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="2d3d9-214">committedContentVersion</span></span>|<span data-ttu-id="2d3d9-215">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="2d3d9-215">String</span></span>|<span data-ttu-id="2d3d9-216">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="2d3d9-216">The internal committed content version.</span></span> <span data-ttu-id="2d3d9-217">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="2d3d9-217">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="2d3d9-218">fileName</span><span class="sxs-lookup"><span data-stu-id="2d3d9-218">fileName</span></span>|<span data-ttu-id="2d3d9-219">String</span><span class="sxs-lookup"><span data-stu-id="2d3d9-219">String</span></span>|<span data-ttu-id="2d3d9-220">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="2d3d9-220">The name of the main Lob application file.</span></span> <span data-ttu-id="2d3d9-221">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="2d3d9-221">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="2d3d9-222">size</span><span class="sxs-lookup"><span data-stu-id="2d3d9-222">size</span></span>|<span data-ttu-id="2d3d9-223">Int64</span><span class="sxs-lookup"><span data-stu-id="2d3d9-223">Int64</span></span>|<span data-ttu-id="2d3d9-224">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="2d3d9-224">The total size, including all uploaded files.</span></span> <span data-ttu-id="2d3d9-225">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="2d3d9-225">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="2d3d9-226">bundleId</span><span class="sxs-lookup"><span data-stu-id="2d3d9-226">bundleId</span></span>|<span data-ttu-id="2d3d9-227">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="2d3d9-227">String</span></span>|<span data-ttu-id="2d3d9-228">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="2d3d9-228">The Identity Name.</span></span>|
|<span data-ttu-id="2d3d9-229">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="2d3d9-229">applicableDeviceType</span></span>|[<span data-ttu-id="2d3d9-230">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="2d3d9-230">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="2d3d9-231">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="2d3d9-231">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="2d3d9-232">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="2d3d9-232">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="2d3d9-233">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="2d3d9-233">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="2d3d9-234">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="2d3d9-234">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="2d3d9-235">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="2d3d9-235">expirationDateTime</span></span>|<span data-ttu-id="2d3d9-236">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d3d9-236">DateTimeOffset</span></span>|<span data-ttu-id="2d3d9-237">O tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="2d3d9-237">The expiration time.</span></span>|
|<span data-ttu-id="2d3d9-238">versionNumber</span><span class="sxs-lookup"><span data-stu-id="2d3d9-238">versionNumber</span></span>|<span data-ttu-id="2d3d9-239">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="2d3d9-239">String</span></span>|<span data-ttu-id="2d3d9-240">O número de versão do aplicativo gerenciado de Linha de Negócios (LoB) iOS gerenciado.</span><span class="sxs-lookup"><span data-stu-id="2d3d9-240">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="2d3d9-241">buildNumber</span><span class="sxs-lookup"><span data-stu-id="2d3d9-241">buildNumber</span></span>|<span data-ttu-id="2d3d9-242">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="2d3d9-242">String</span></span>|<span data-ttu-id="2d3d9-243">O número de build do aplicativo gerenciado de Linha de Negócios (LoB) iOS gerenciado.</span><span class="sxs-lookup"><span data-stu-id="2d3d9-243">The build number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="2d3d9-244">identityVersion</span><span class="sxs-lookup"><span data-stu-id="2d3d9-244">identityVersion</span></span>|<span data-ttu-id="2d3d9-245">String</span><span class="sxs-lookup"><span data-stu-id="2d3d9-245">String</span></span>|<span data-ttu-id="2d3d9-246">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="2d3d9-246">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="2d3d9-247">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d3d9-247">Response</span></span>
<span data-ttu-id="2d3d9-248">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2d3d9-248">If successful, this method returns a `200 OK` response code and an updated [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d3d9-249">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2d3d9-249">Example</span></span>

### <a name="request"></a><span data-ttu-id="2d3d9-250">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2d3d9-250">Request</span></span>
<span data-ttu-id="2d3d9-251">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2d3d9-251">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1489

{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "bundleId": "Bundle Id value",
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
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="2d3d9-252">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d3d9-252">Response</span></span>
<span data-ttu-id="2d3d9-p124">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2d3d9-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1661

{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
  "id": "8f59792d-792d-8f59-2d79-598f2d79598f",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "bundleId": "Bundle Id value",
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
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```





