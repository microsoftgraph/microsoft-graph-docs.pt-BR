---
title: Atualizar managedIOSLobApp
description: Atualiza as propriedades de um objeto managedIOSLobApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2f8da4cc926c4425d8b483526de1a397ef07eca1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42445082"
---
# <a name="update-managedioslobapp"></a><span data-ttu-id="d3c81-103">Atualizar managedIOSLobApp</span><span class="sxs-lookup"><span data-stu-id="d3c81-103">Update managedIOSLobApp</span></span>

<span data-ttu-id="d3c81-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d3c81-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d3c81-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d3c81-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d3c81-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d3c81-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3c81-107">Atualiza as propriedades de um objeto [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="d3c81-107">Update the properties of a [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d3c81-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d3c81-108">Prerequisites</span></span>
<span data-ttu-id="d3c81-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3c81-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3c81-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d3c81-111">Permission type</span></span>|<span data-ttu-id="d3c81-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d3c81-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3c81-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d3c81-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d3c81-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3c81-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d3c81-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d3c81-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3c81-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3c81-116">Not supported.</span></span>|
|<span data-ttu-id="d3c81-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d3c81-117">Application</span></span>|<span data-ttu-id="d3c81-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3c81-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3c81-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d3c81-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="d3c81-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d3c81-120">Request headers</span></span>
|<span data-ttu-id="d3c81-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d3c81-121">Header</span></span>|<span data-ttu-id="d3c81-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d3c81-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d3c81-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d3c81-123">Authorization</span></span>|<span data-ttu-id="d3c81-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d3c81-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d3c81-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d3c81-125">Accept</span></span>|<span data-ttu-id="d3c81-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d3c81-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3c81-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d3c81-127">Request body</span></span>
<span data-ttu-id="d3c81-128">No corpo da solicitação, forneça uma representação JSON do objeto [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="d3c81-128">In the request body, supply a JSON representation for the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

<span data-ttu-id="d3c81-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="d3c81-129">The following table shows the properties that are required when you create the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span></span>

|<span data-ttu-id="d3c81-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d3c81-130">Property</span></span>|<span data-ttu-id="d3c81-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d3c81-131">Type</span></span>|<span data-ttu-id="d3c81-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3c81-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3c81-133">id</span><span class="sxs-lookup"><span data-stu-id="d3c81-133">id</span></span>|<span data-ttu-id="d3c81-134">String</span><span class="sxs-lookup"><span data-stu-id="d3c81-134">String</span></span>|<span data-ttu-id="d3c81-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d3c81-135">Key of the entity.</span></span> <span data-ttu-id="d3c81-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d3c81-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d3c81-137">displayName</span><span class="sxs-lookup"><span data-stu-id="d3c81-137">displayName</span></span>|<span data-ttu-id="d3c81-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d3c81-138">String</span></span>|<span data-ttu-id="d3c81-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="d3c81-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="d3c81-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d3c81-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d3c81-141">description</span><span class="sxs-lookup"><span data-stu-id="d3c81-141">description</span></span>|<span data-ttu-id="d3c81-142">String</span><span class="sxs-lookup"><span data-stu-id="d3c81-142">String</span></span>|<span data-ttu-id="d3c81-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d3c81-143">The description of the app.</span></span> <span data-ttu-id="d3c81-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d3c81-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d3c81-145">publicador</span><span class="sxs-lookup"><span data-stu-id="d3c81-145">publisher</span></span>|<span data-ttu-id="d3c81-146">String</span><span class="sxs-lookup"><span data-stu-id="d3c81-146">String</span></span>|<span data-ttu-id="d3c81-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d3c81-147">The publisher of the app.</span></span> <span data-ttu-id="d3c81-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d3c81-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d3c81-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="d3c81-149">largeIcon</span></span>|[<span data-ttu-id="d3c81-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="d3c81-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="d3c81-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="d3c81-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="d3c81-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d3c81-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d3c81-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d3c81-153">createdDateTime</span></span>|<span data-ttu-id="d3c81-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3c81-154">DateTimeOffset</span></span>|<span data-ttu-id="d3c81-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d3c81-155">The date and time the app was created.</span></span> <span data-ttu-id="d3c81-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d3c81-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d3c81-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d3c81-157">lastModifiedDateTime</span></span>|<span data-ttu-id="d3c81-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3c81-158">DateTimeOffset</span></span>|<span data-ttu-id="d3c81-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="d3c81-159">The date and time the app was last modified.</span></span> <span data-ttu-id="d3c81-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d3c81-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d3c81-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="d3c81-161">isFeatured</span></span>|<span data-ttu-id="d3c81-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="d3c81-162">Boolean</span></span>|<span data-ttu-id="d3c81-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d3c81-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d3c81-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="d3c81-164">privacyInformationUrl</span></span>|<span data-ttu-id="d3c81-165">String</span><span class="sxs-lookup"><span data-stu-id="d3c81-165">String</span></span>|<span data-ttu-id="d3c81-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="d3c81-166">The privacy statement Url.</span></span> <span data-ttu-id="d3c81-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d3c81-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d3c81-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="d3c81-168">informationUrl</span></span>|<span data-ttu-id="d3c81-169">String</span><span class="sxs-lookup"><span data-stu-id="d3c81-169">String</span></span>|<span data-ttu-id="d3c81-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="d3c81-170">The more information Url.</span></span> <span data-ttu-id="d3c81-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d3c81-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d3c81-172">owner</span><span class="sxs-lookup"><span data-stu-id="d3c81-172">owner</span></span>|<span data-ttu-id="d3c81-173">String</span><span class="sxs-lookup"><span data-stu-id="d3c81-173">String</span></span>|<span data-ttu-id="d3c81-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="d3c81-174">The owner of the app.</span></span> <span data-ttu-id="d3c81-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d3c81-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d3c81-176">developer</span><span class="sxs-lookup"><span data-stu-id="d3c81-176">developer</span></span>|<span data-ttu-id="d3c81-177">String</span><span class="sxs-lookup"><span data-stu-id="d3c81-177">String</span></span>|<span data-ttu-id="d3c81-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d3c81-178">The developer of the app.</span></span> <span data-ttu-id="d3c81-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d3c81-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d3c81-180">notes</span><span class="sxs-lookup"><span data-stu-id="d3c81-180">notes</span></span>|<span data-ttu-id="d3c81-181">String</span><span class="sxs-lookup"><span data-stu-id="d3c81-181">String</span></span>|<span data-ttu-id="d3c81-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d3c81-182">Notes for the app.</span></span> <span data-ttu-id="d3c81-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d3c81-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d3c81-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="d3c81-184">uploadState</span></span>|<span data-ttu-id="d3c81-185">Int32</span><span class="sxs-lookup"><span data-stu-id="d3c81-185">Int32</span></span>|<span data-ttu-id="d3c81-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="d3c81-186">The upload state.</span></span> <span data-ttu-id="d3c81-187">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d3c81-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d3c81-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="d3c81-188">publishingState</span></span>|[<span data-ttu-id="d3c81-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="d3c81-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="d3c81-190">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d3c81-190">The publishing state for the app.</span></span> <span data-ttu-id="d3c81-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="d3c81-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="d3c81-192">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d3c81-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="d3c81-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="d3c81-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="d3c81-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="d3c81-194">isAssigned</span></span>|<span data-ttu-id="d3c81-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="d3c81-195">Boolean</span></span>|<span data-ttu-id="d3c81-196">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="d3c81-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="d3c81-197">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d3c81-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d3c81-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d3c81-198">roleScopeTagIds</span></span>|<span data-ttu-id="d3c81-199">String collection</span><span class="sxs-lookup"><span data-stu-id="d3c81-199">String collection</span></span>|<span data-ttu-id="d3c81-200">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="d3c81-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="d3c81-201">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d3c81-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d3c81-202">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="d3c81-202">dependentAppCount</span></span>|<span data-ttu-id="d3c81-203">Int32</span><span class="sxs-lookup"><span data-stu-id="d3c81-203">Int32</span></span>|<span data-ttu-id="d3c81-204">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="d3c81-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="d3c81-205">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d3c81-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d3c81-206">appAvailability</span><span class="sxs-lookup"><span data-stu-id="d3c81-206">appAvailability</span></span>|[<span data-ttu-id="d3c81-207">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="d3c81-207">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="d3c81-208">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d3c81-208">The Application's availability.</span></span> <span data-ttu-id="d3c81-209">Herdado de [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="d3c81-209">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="d3c81-210">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="d3c81-210">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="d3c81-211">version</span><span class="sxs-lookup"><span data-stu-id="d3c81-211">version</span></span>|<span data-ttu-id="d3c81-212">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d3c81-212">String</span></span>|<span data-ttu-id="d3c81-213">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d3c81-213">The Application's version.</span></span> <span data-ttu-id="d3c81-214">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="d3c81-214">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="d3c81-215">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="d3c81-215">committedContentVersion</span></span>|<span data-ttu-id="d3c81-216">String</span><span class="sxs-lookup"><span data-stu-id="d3c81-216">String</span></span>|<span data-ttu-id="d3c81-217">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="d3c81-217">The internal committed content version.</span></span> <span data-ttu-id="d3c81-218">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="d3c81-218">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="d3c81-219">fileName</span><span class="sxs-lookup"><span data-stu-id="d3c81-219">fileName</span></span>|<span data-ttu-id="d3c81-220">String</span><span class="sxs-lookup"><span data-stu-id="d3c81-220">String</span></span>|<span data-ttu-id="d3c81-221">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="d3c81-221">The name of the main Lob application file.</span></span> <span data-ttu-id="d3c81-222">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="d3c81-222">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="d3c81-223">size</span><span class="sxs-lookup"><span data-stu-id="d3c81-223">size</span></span>|<span data-ttu-id="d3c81-224">Int64</span><span class="sxs-lookup"><span data-stu-id="d3c81-224">Int64</span></span>|<span data-ttu-id="d3c81-225">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="d3c81-225">The total size, including all uploaded files.</span></span> <span data-ttu-id="d3c81-226">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="d3c81-226">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="d3c81-227">bundleId</span><span class="sxs-lookup"><span data-stu-id="d3c81-227">bundleId</span></span>|<span data-ttu-id="d3c81-228">String</span><span class="sxs-lookup"><span data-stu-id="d3c81-228">String</span></span>|<span data-ttu-id="d3c81-229">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="d3c81-229">The Identity Name.</span></span>|
|<span data-ttu-id="d3c81-230">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="d3c81-230">applicableDeviceType</span></span>|[<span data-ttu-id="d3c81-231">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="d3c81-231">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="d3c81-232">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="d3c81-232">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="d3c81-233">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="d3c81-233">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="d3c81-234">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="d3c81-234">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="d3c81-235">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="d3c81-235">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="d3c81-236">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="d3c81-236">expirationDateTime</span></span>|<span data-ttu-id="d3c81-237">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3c81-237">DateTimeOffset</span></span>|<span data-ttu-id="d3c81-238">O tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="d3c81-238">The expiration time.</span></span>|
|<span data-ttu-id="d3c81-239">versionNumber</span><span class="sxs-lookup"><span data-stu-id="d3c81-239">versionNumber</span></span>|<span data-ttu-id="d3c81-240">String</span><span class="sxs-lookup"><span data-stu-id="d3c81-240">String</span></span>|<span data-ttu-id="d3c81-241">O número de versão do aplicativo gerenciado de Linha de Negócios (LoB) iOS gerenciado.</span><span class="sxs-lookup"><span data-stu-id="d3c81-241">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="d3c81-242">buildNumber</span><span class="sxs-lookup"><span data-stu-id="d3c81-242">buildNumber</span></span>|<span data-ttu-id="d3c81-243">String</span><span class="sxs-lookup"><span data-stu-id="d3c81-243">String</span></span>|<span data-ttu-id="d3c81-244">O número de build do aplicativo gerenciado de Linha de Negócios (LoB) iOS gerenciado.</span><span class="sxs-lookup"><span data-stu-id="d3c81-244">The build number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="d3c81-245">identityVersion</span><span class="sxs-lookup"><span data-stu-id="d3c81-245">identityVersion</span></span>|<span data-ttu-id="d3c81-246">String</span><span class="sxs-lookup"><span data-stu-id="d3c81-246">String</span></span>|<span data-ttu-id="d3c81-247">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="d3c81-247">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="d3c81-248">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3c81-248">Response</span></span>
<span data-ttu-id="d3c81-249">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d3c81-249">If successful, this method returns a `200 OK` response code and an updated [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3c81-250">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d3c81-250">Example</span></span>

### <a name="request"></a><span data-ttu-id="d3c81-251">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d3c81-251">Request</span></span>
<span data-ttu-id="d3c81-252">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d3c81-252">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d3c81-253">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3c81-253">Response</span></span>
<span data-ttu-id="d3c81-p124">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d3c81-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





