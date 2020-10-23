---
title: Criar managedIOSLobApp
description: Cria um novo objeto managedIOSLobApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 63037b12308839d8c8764d4555b77e14ad6da21e
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48699300"
---
# <a name="create-managedioslobapp"></a><span data-ttu-id="f7725-103">Criar managedIOSLobApp</span><span class="sxs-lookup"><span data-stu-id="f7725-103">Create managedIOSLobApp</span></span>

<span data-ttu-id="f7725-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7725-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f7725-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f7725-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f7725-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f7725-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7725-107">Cria um novo objeto [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="f7725-107">Create a new [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f7725-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f7725-108">Prerequisites</span></span>
<span data-ttu-id="f7725-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7725-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7725-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f7725-111">Permission type</span></span>|<span data-ttu-id="f7725-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f7725-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f7725-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f7725-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f7725-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7725-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f7725-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f7725-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7725-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f7725-116">Not supported.</span></span>|
|<span data-ttu-id="f7725-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f7725-117">Application</span></span>|<span data-ttu-id="f7725-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7725-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f7725-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f7725-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="f7725-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f7725-120">Request headers</span></span>
|<span data-ttu-id="f7725-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f7725-121">Header</span></span>|<span data-ttu-id="f7725-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f7725-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f7725-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f7725-123">Authorization</span></span>|<span data-ttu-id="f7725-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f7725-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f7725-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f7725-125">Accept</span></span>|<span data-ttu-id="f7725-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f7725-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7725-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f7725-127">Request body</span></span>
<span data-ttu-id="f7725-128">No corpo da solicitação, forneça uma representação JSON do objeto managedIOSLobApp.</span><span class="sxs-lookup"><span data-stu-id="f7725-128">In the request body, supply a JSON representation for the managedIOSLobApp object.</span></span>

<span data-ttu-id="f7725-129">A tabela a seguir mostra as propriedades obrigatórias ao criar managedIOSLobApp.</span><span class="sxs-lookup"><span data-stu-id="f7725-129">The following table shows the properties that are required when you create the managedIOSLobApp.</span></span>

|<span data-ttu-id="f7725-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f7725-130">Property</span></span>|<span data-ttu-id="f7725-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f7725-131">Type</span></span>|<span data-ttu-id="f7725-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7725-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7725-133">id</span><span class="sxs-lookup"><span data-stu-id="f7725-133">id</span></span>|<span data-ttu-id="f7725-134">String</span><span class="sxs-lookup"><span data-stu-id="f7725-134">String</span></span>|<span data-ttu-id="f7725-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f7725-135">Key of the entity.</span></span> <span data-ttu-id="f7725-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f7725-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f7725-137">displayName</span><span class="sxs-lookup"><span data-stu-id="f7725-137">displayName</span></span>|<span data-ttu-id="f7725-138">String</span><span class="sxs-lookup"><span data-stu-id="f7725-138">String</span></span>|<span data-ttu-id="f7725-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="f7725-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="f7725-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f7725-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f7725-141">description</span><span class="sxs-lookup"><span data-stu-id="f7725-141">description</span></span>|<span data-ttu-id="f7725-142">String</span><span class="sxs-lookup"><span data-stu-id="f7725-142">String</span></span>|<span data-ttu-id="f7725-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f7725-143">The description of the app.</span></span> <span data-ttu-id="f7725-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f7725-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f7725-145">publicador</span><span class="sxs-lookup"><span data-stu-id="f7725-145">publisher</span></span>|<span data-ttu-id="f7725-146">String</span><span class="sxs-lookup"><span data-stu-id="f7725-146">String</span></span>|<span data-ttu-id="f7725-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f7725-147">The publisher of the app.</span></span> <span data-ttu-id="f7725-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f7725-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f7725-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="f7725-149">largeIcon</span></span>|[<span data-ttu-id="f7725-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f7725-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f7725-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="f7725-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="f7725-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f7725-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f7725-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f7725-153">createdDateTime</span></span>|<span data-ttu-id="f7725-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7725-154">DateTimeOffset</span></span>|<span data-ttu-id="f7725-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f7725-155">The date and time the app was created.</span></span> <span data-ttu-id="f7725-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f7725-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f7725-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f7725-157">lastModifiedDateTime</span></span>|<span data-ttu-id="f7725-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7725-158">DateTimeOffset</span></span>|<span data-ttu-id="f7725-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="f7725-159">The date and time the app was last modified.</span></span> <span data-ttu-id="f7725-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f7725-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f7725-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="f7725-161">isFeatured</span></span>|<span data-ttu-id="f7725-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="f7725-162">Boolean</span></span>|<span data-ttu-id="f7725-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f7725-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f7725-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f7725-164">privacyInformationUrl</span></span>|<span data-ttu-id="f7725-165">String</span><span class="sxs-lookup"><span data-stu-id="f7725-165">String</span></span>|<span data-ttu-id="f7725-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="f7725-166">The privacy statement Url.</span></span> <span data-ttu-id="f7725-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f7725-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f7725-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f7725-168">informationUrl</span></span>|<span data-ttu-id="f7725-169">String</span><span class="sxs-lookup"><span data-stu-id="f7725-169">String</span></span>|<span data-ttu-id="f7725-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="f7725-170">The more information Url.</span></span> <span data-ttu-id="f7725-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f7725-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f7725-172">owner</span><span class="sxs-lookup"><span data-stu-id="f7725-172">owner</span></span>|<span data-ttu-id="f7725-173">String</span><span class="sxs-lookup"><span data-stu-id="f7725-173">String</span></span>|<span data-ttu-id="f7725-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="f7725-174">The owner of the app.</span></span> <span data-ttu-id="f7725-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f7725-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f7725-176">developer</span><span class="sxs-lookup"><span data-stu-id="f7725-176">developer</span></span>|<span data-ttu-id="f7725-177">String</span><span class="sxs-lookup"><span data-stu-id="f7725-177">String</span></span>|<span data-ttu-id="f7725-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f7725-178">The developer of the app.</span></span> <span data-ttu-id="f7725-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f7725-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f7725-180">notes</span><span class="sxs-lookup"><span data-stu-id="f7725-180">notes</span></span>|<span data-ttu-id="f7725-181">String</span><span class="sxs-lookup"><span data-stu-id="f7725-181">String</span></span>|<span data-ttu-id="f7725-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f7725-182">Notes for the app.</span></span> <span data-ttu-id="f7725-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f7725-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f7725-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="f7725-184">uploadState</span></span>|<span data-ttu-id="f7725-185">Int32</span><span class="sxs-lookup"><span data-stu-id="f7725-185">Int32</span></span>|<span data-ttu-id="f7725-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="f7725-186">The upload state.</span></span> <span data-ttu-id="f7725-187">Os valores possíveis são: 0- `Not Ready` , 1- `Ready` , 2- `Processing` .</span><span class="sxs-lookup"><span data-stu-id="f7725-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="f7725-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f7725-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f7725-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="f7725-189">publishingState</span></span>|[<span data-ttu-id="f7725-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="f7725-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="f7725-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f7725-191">The publishing state for the app.</span></span> <span data-ttu-id="f7725-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="f7725-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="f7725-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f7725-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="f7725-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="f7725-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="f7725-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="f7725-195">isAssigned</span></span>|<span data-ttu-id="f7725-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="f7725-196">Boolean</span></span>|<span data-ttu-id="f7725-197">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="f7725-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="f7725-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f7725-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f7725-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f7725-199">roleScopeTagIds</span></span>|<span data-ttu-id="f7725-200">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f7725-200">String collection</span></span>|<span data-ttu-id="f7725-201">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="f7725-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="f7725-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f7725-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f7725-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="f7725-203">dependentAppCount</span></span>|<span data-ttu-id="f7725-204">Int32</span><span class="sxs-lookup"><span data-stu-id="f7725-204">Int32</span></span>|<span data-ttu-id="f7725-205">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="f7725-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="f7725-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f7725-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f7725-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="f7725-207">supersedingAppCount</span></span>|<span data-ttu-id="f7725-208">Int32</span><span class="sxs-lookup"><span data-stu-id="f7725-208">Int32</span></span>|<span data-ttu-id="f7725-209">O número total de aplicativos que este aplicativo substitui direta ou indiretamente.</span><span class="sxs-lookup"><span data-stu-id="f7725-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="f7725-210">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f7725-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f7725-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="f7725-211">supersededAppCount</span></span>|<span data-ttu-id="f7725-212">Int32</span><span class="sxs-lookup"><span data-stu-id="f7725-212">Int32</span></span>|<span data-ttu-id="f7725-213">O número total de aplicativos que este aplicativo está substituindo direta ou indiretamente por.</span><span class="sxs-lookup"><span data-stu-id="f7725-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="f7725-214">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f7725-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f7725-215">appAvailability</span><span class="sxs-lookup"><span data-stu-id="f7725-215">appAvailability</span></span>|[<span data-ttu-id="f7725-216">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="f7725-216">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="f7725-217">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f7725-217">The Application's availability.</span></span> <span data-ttu-id="f7725-218">Herdado de [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="f7725-218">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="f7725-219">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="f7725-219">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="f7725-220">version</span><span class="sxs-lookup"><span data-stu-id="f7725-220">version</span></span>|<span data-ttu-id="f7725-221">String</span><span class="sxs-lookup"><span data-stu-id="f7725-221">String</span></span>|<span data-ttu-id="f7725-222">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f7725-222">The Application's version.</span></span> <span data-ttu-id="f7725-223">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="f7725-223">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="f7725-224">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="f7725-224">committedContentVersion</span></span>|<span data-ttu-id="f7725-225">String</span><span class="sxs-lookup"><span data-stu-id="f7725-225">String</span></span>|<span data-ttu-id="f7725-226">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="f7725-226">The internal committed content version.</span></span> <span data-ttu-id="f7725-227">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="f7725-227">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="f7725-228">fileName</span><span class="sxs-lookup"><span data-stu-id="f7725-228">fileName</span></span>|<span data-ttu-id="f7725-229">String</span><span class="sxs-lookup"><span data-stu-id="f7725-229">String</span></span>|<span data-ttu-id="f7725-230">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="f7725-230">The name of the main Lob application file.</span></span> <span data-ttu-id="f7725-231">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="f7725-231">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="f7725-232">size</span><span class="sxs-lookup"><span data-stu-id="f7725-232">size</span></span>|<span data-ttu-id="f7725-233">Int64</span><span class="sxs-lookup"><span data-stu-id="f7725-233">Int64</span></span>|<span data-ttu-id="f7725-234">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="f7725-234">The total size, including all uploaded files.</span></span> <span data-ttu-id="f7725-235">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="f7725-235">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="f7725-236">bundleId</span><span class="sxs-lookup"><span data-stu-id="f7725-236">bundleId</span></span>|<span data-ttu-id="f7725-237">String</span><span class="sxs-lookup"><span data-stu-id="f7725-237">String</span></span>|<span data-ttu-id="f7725-238">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="f7725-238">The Identity Name.</span></span>|
|<span data-ttu-id="f7725-239">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="f7725-239">applicableDeviceType</span></span>|[<span data-ttu-id="f7725-240">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="f7725-240">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="f7725-241">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="f7725-241">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="f7725-242">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f7725-242">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="f7725-243">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f7725-243">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="f7725-244">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="f7725-244">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="f7725-245">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f7725-245">expirationDateTime</span></span>|<span data-ttu-id="f7725-246">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7725-246">DateTimeOffset</span></span>|<span data-ttu-id="f7725-247">O tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="f7725-247">The expiration time.</span></span>|
|<span data-ttu-id="f7725-248">versionNumber</span><span class="sxs-lookup"><span data-stu-id="f7725-248">versionNumber</span></span>|<span data-ttu-id="f7725-249">String</span><span class="sxs-lookup"><span data-stu-id="f7725-249">String</span></span>|<span data-ttu-id="f7725-250">O número de versão do aplicativo gerenciado de Linha de Negócios (LoB) iOS gerenciado.</span><span class="sxs-lookup"><span data-stu-id="f7725-250">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="f7725-251">buildNumber</span><span class="sxs-lookup"><span data-stu-id="f7725-251">buildNumber</span></span>|<span data-ttu-id="f7725-252">String</span><span class="sxs-lookup"><span data-stu-id="f7725-252">String</span></span>|<span data-ttu-id="f7725-253">O número de build do aplicativo gerenciado de Linha de Negócios (LoB) iOS gerenciado.</span><span class="sxs-lookup"><span data-stu-id="f7725-253">The build number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="f7725-254">identityVersion</span><span class="sxs-lookup"><span data-stu-id="f7725-254">identityVersion</span></span>|<span data-ttu-id="f7725-255">String</span><span class="sxs-lookup"><span data-stu-id="f7725-255">String</span></span>|<span data-ttu-id="f7725-256">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="f7725-256">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="f7725-257">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7725-257">Response</span></span>
<span data-ttu-id="f7725-258">Se tiver êxito, este método retornará o código de resposta `201 Created` e o objeto [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f7725-258">If successful, this method returns a `201 Created` response code and a [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7725-259">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f7725-259">Example</span></span>

### <a name="request"></a><span data-ttu-id="f7725-260">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f7725-260">Request</span></span>
<span data-ttu-id="f7725-261">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f7725-261">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1546

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
  "supersedingAppCount": 3,
  "supersededAppCount": 2,
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

### <a name="response"></a><span data-ttu-id="f7725-262">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7725-262">Response</span></span>
<span data-ttu-id="f7725-p126">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f7725-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1718

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
  "supersedingAppCount": 3,
  "supersededAppCount": 2,
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





