---
title: Criar managedAndroidLobApp
description: Cria um novo objeto managedAndroidLobApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a6056d7ccecf0edb66446f36b61e25a126a0b23b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49250846"
---
# <a name="create-managedandroidlobapp"></a><span data-ttu-id="4076f-103">Criar managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="4076f-103">Create managedAndroidLobApp</span></span>

<span data-ttu-id="4076f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4076f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4076f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4076f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4076f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4076f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4076f-107">Cria um novo objeto [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="4076f-107">Create a new [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4076f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4076f-108">Prerequisites</span></span>
<span data-ttu-id="4076f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4076f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4076f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4076f-111">Permission type</span></span>|<span data-ttu-id="4076f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4076f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4076f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4076f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4076f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4076f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4076f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4076f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4076f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4076f-116">Not supported.</span></span>|
|<span data-ttu-id="4076f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4076f-117">Application</span></span>|<span data-ttu-id="4076f-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4076f-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4076f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4076f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="4076f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4076f-120">Request headers</span></span>
|<span data-ttu-id="4076f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4076f-121">Header</span></span>|<span data-ttu-id="4076f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4076f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4076f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4076f-123">Authorization</span></span>|<span data-ttu-id="4076f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4076f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4076f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4076f-125">Accept</span></span>|<span data-ttu-id="4076f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4076f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4076f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4076f-127">Request body</span></span>
<span data-ttu-id="4076f-128">No corpo da solicitação, forneça uma representação JSON do objeto managedAndroidLobApp.</span><span class="sxs-lookup"><span data-stu-id="4076f-128">In the request body, supply a JSON representation for the managedAndroidLobApp object.</span></span>

<span data-ttu-id="4076f-129">A tabela a seguir mostra as propriedades obrigatórias ao criar managedAndroidLobApp.</span><span class="sxs-lookup"><span data-stu-id="4076f-129">The following table shows the properties that are required when you create the managedAndroidLobApp.</span></span>

|<span data-ttu-id="4076f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4076f-130">Property</span></span>|<span data-ttu-id="4076f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4076f-131">Type</span></span>|<span data-ttu-id="4076f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4076f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4076f-133">id</span><span class="sxs-lookup"><span data-stu-id="4076f-133">id</span></span>|<span data-ttu-id="4076f-134">String</span><span class="sxs-lookup"><span data-stu-id="4076f-134">String</span></span>|<span data-ttu-id="4076f-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4076f-135">Key of the entity.</span></span> <span data-ttu-id="4076f-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4076f-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4076f-137">displayName</span><span class="sxs-lookup"><span data-stu-id="4076f-137">displayName</span></span>|<span data-ttu-id="4076f-138">String</span><span class="sxs-lookup"><span data-stu-id="4076f-138">String</span></span>|<span data-ttu-id="4076f-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="4076f-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="4076f-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4076f-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4076f-141">description</span><span class="sxs-lookup"><span data-stu-id="4076f-141">description</span></span>|<span data-ttu-id="4076f-142">String</span><span class="sxs-lookup"><span data-stu-id="4076f-142">String</span></span>|<span data-ttu-id="4076f-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4076f-143">The description of the app.</span></span> <span data-ttu-id="4076f-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4076f-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4076f-145">publicador</span><span class="sxs-lookup"><span data-stu-id="4076f-145">publisher</span></span>|<span data-ttu-id="4076f-146">String</span><span class="sxs-lookup"><span data-stu-id="4076f-146">String</span></span>|<span data-ttu-id="4076f-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4076f-147">The publisher of the app.</span></span> <span data-ttu-id="4076f-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4076f-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4076f-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="4076f-149">largeIcon</span></span>|[<span data-ttu-id="4076f-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="4076f-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="4076f-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="4076f-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="4076f-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4076f-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4076f-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4076f-153">createdDateTime</span></span>|<span data-ttu-id="4076f-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4076f-154">DateTimeOffset</span></span>|<span data-ttu-id="4076f-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4076f-155">The date and time the app was created.</span></span> <span data-ttu-id="4076f-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4076f-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4076f-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4076f-157">lastModifiedDateTime</span></span>|<span data-ttu-id="4076f-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4076f-158">DateTimeOffset</span></span>|<span data-ttu-id="4076f-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="4076f-159">The date and time the app was last modified.</span></span> <span data-ttu-id="4076f-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4076f-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4076f-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="4076f-161">isFeatured</span></span>|<span data-ttu-id="4076f-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="4076f-162">Boolean</span></span>|<span data-ttu-id="4076f-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4076f-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4076f-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="4076f-164">privacyInformationUrl</span></span>|<span data-ttu-id="4076f-165">String</span><span class="sxs-lookup"><span data-stu-id="4076f-165">String</span></span>|<span data-ttu-id="4076f-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="4076f-166">The privacy statement Url.</span></span> <span data-ttu-id="4076f-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4076f-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4076f-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="4076f-168">informationUrl</span></span>|<span data-ttu-id="4076f-169">String</span><span class="sxs-lookup"><span data-stu-id="4076f-169">String</span></span>|<span data-ttu-id="4076f-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="4076f-170">The more information Url.</span></span> <span data-ttu-id="4076f-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4076f-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4076f-172">owner</span><span class="sxs-lookup"><span data-stu-id="4076f-172">owner</span></span>|<span data-ttu-id="4076f-173">String</span><span class="sxs-lookup"><span data-stu-id="4076f-173">String</span></span>|<span data-ttu-id="4076f-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="4076f-174">The owner of the app.</span></span> <span data-ttu-id="4076f-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4076f-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4076f-176">developer</span><span class="sxs-lookup"><span data-stu-id="4076f-176">developer</span></span>|<span data-ttu-id="4076f-177">String</span><span class="sxs-lookup"><span data-stu-id="4076f-177">String</span></span>|<span data-ttu-id="4076f-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4076f-178">The developer of the app.</span></span> <span data-ttu-id="4076f-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4076f-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4076f-180">notes</span><span class="sxs-lookup"><span data-stu-id="4076f-180">notes</span></span>|<span data-ttu-id="4076f-181">String</span><span class="sxs-lookup"><span data-stu-id="4076f-181">String</span></span>|<span data-ttu-id="4076f-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4076f-182">Notes for the app.</span></span> <span data-ttu-id="4076f-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4076f-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4076f-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="4076f-184">uploadState</span></span>|<span data-ttu-id="4076f-185">Int32</span><span class="sxs-lookup"><span data-stu-id="4076f-185">Int32</span></span>|<span data-ttu-id="4076f-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="4076f-186">The upload state.</span></span> <span data-ttu-id="4076f-187">Os valores possíveis são: 0- `Not Ready` , 1- `Ready` , 2- `Processing` .</span><span class="sxs-lookup"><span data-stu-id="4076f-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="4076f-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4076f-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4076f-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="4076f-189">publishingState</span></span>|[<span data-ttu-id="4076f-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="4076f-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="4076f-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4076f-191">The publishing state for the app.</span></span> <span data-ttu-id="4076f-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="4076f-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="4076f-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4076f-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="4076f-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="4076f-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="4076f-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="4076f-195">isAssigned</span></span>|<span data-ttu-id="4076f-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="4076f-196">Boolean</span></span>|<span data-ttu-id="4076f-197">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="4076f-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="4076f-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4076f-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4076f-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4076f-199">roleScopeTagIds</span></span>|<span data-ttu-id="4076f-200">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="4076f-200">String collection</span></span>|<span data-ttu-id="4076f-201">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="4076f-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="4076f-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4076f-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4076f-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="4076f-203">dependentAppCount</span></span>|<span data-ttu-id="4076f-204">Int32</span><span class="sxs-lookup"><span data-stu-id="4076f-204">Int32</span></span>|<span data-ttu-id="4076f-205">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="4076f-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="4076f-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4076f-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4076f-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="4076f-207">supersedingAppCount</span></span>|<span data-ttu-id="4076f-208">Int32</span><span class="sxs-lookup"><span data-stu-id="4076f-208">Int32</span></span>|<span data-ttu-id="4076f-209">O número total de aplicativos que este aplicativo substitui direta ou indiretamente.</span><span class="sxs-lookup"><span data-stu-id="4076f-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="4076f-210">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4076f-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4076f-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="4076f-211">supersededAppCount</span></span>|<span data-ttu-id="4076f-212">Int32</span><span class="sxs-lookup"><span data-stu-id="4076f-212">Int32</span></span>|<span data-ttu-id="4076f-213">O número total de aplicativos que este aplicativo está substituindo direta ou indiretamente por.</span><span class="sxs-lookup"><span data-stu-id="4076f-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="4076f-214">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4076f-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4076f-215">appAvailability</span><span class="sxs-lookup"><span data-stu-id="4076f-215">appAvailability</span></span>|[<span data-ttu-id="4076f-216">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="4076f-216">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="4076f-217">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4076f-217">The Application's availability.</span></span> <span data-ttu-id="4076f-218">Herdado de [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="4076f-218">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="4076f-219">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="4076f-219">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="4076f-220">version</span><span class="sxs-lookup"><span data-stu-id="4076f-220">version</span></span>|<span data-ttu-id="4076f-221">String</span><span class="sxs-lookup"><span data-stu-id="4076f-221">String</span></span>|<span data-ttu-id="4076f-222">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4076f-222">The Application's version.</span></span> <span data-ttu-id="4076f-223">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="4076f-223">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="4076f-224">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="4076f-224">committedContentVersion</span></span>|<span data-ttu-id="4076f-225">String</span><span class="sxs-lookup"><span data-stu-id="4076f-225">String</span></span>|<span data-ttu-id="4076f-226">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="4076f-226">The internal committed content version.</span></span> <span data-ttu-id="4076f-227">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="4076f-227">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="4076f-228">fileName</span><span class="sxs-lookup"><span data-stu-id="4076f-228">fileName</span></span>|<span data-ttu-id="4076f-229">String</span><span class="sxs-lookup"><span data-stu-id="4076f-229">String</span></span>|<span data-ttu-id="4076f-230">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="4076f-230">The name of the main Lob application file.</span></span> <span data-ttu-id="4076f-231">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="4076f-231">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="4076f-232">size</span><span class="sxs-lookup"><span data-stu-id="4076f-232">size</span></span>|<span data-ttu-id="4076f-233">Int64</span><span class="sxs-lookup"><span data-stu-id="4076f-233">Int64</span></span>|<span data-ttu-id="4076f-234">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="4076f-234">The total size, including all uploaded files.</span></span> <span data-ttu-id="4076f-235">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="4076f-235">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="4076f-236">packageId</span><span class="sxs-lookup"><span data-stu-id="4076f-236">packageId</span></span>|<span data-ttu-id="4076f-237">String</span><span class="sxs-lookup"><span data-stu-id="4076f-237">String</span></span>|<span data-ttu-id="4076f-238">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="4076f-238">The package identifier.</span></span>|
|<span data-ttu-id="4076f-239">identityName</span><span class="sxs-lookup"><span data-stu-id="4076f-239">identityName</span></span>|<span data-ttu-id="4076f-240">String</span><span class="sxs-lookup"><span data-stu-id="4076f-240">String</span></span>|<span data-ttu-id="4076f-241">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="4076f-241">The Identity Name.</span></span>|
|<span data-ttu-id="4076f-242">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="4076f-242">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="4076f-243">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="4076f-243">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="4076f-244">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="4076f-244">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="4076f-245">versionName</span><span class="sxs-lookup"><span data-stu-id="4076f-245">versionName</span></span>|<span data-ttu-id="4076f-246">String</span><span class="sxs-lookup"><span data-stu-id="4076f-246">String</span></span>|<span data-ttu-id="4076f-247">O nome da versão do aplicativo gerenciado de Linha de Negócios (LoB) Android gerenciado.</span><span class="sxs-lookup"><span data-stu-id="4076f-247">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="4076f-248">versionCode</span><span class="sxs-lookup"><span data-stu-id="4076f-248">versionCode</span></span>|<span data-ttu-id="4076f-249">String</span><span class="sxs-lookup"><span data-stu-id="4076f-249">String</span></span>|<span data-ttu-id="4076f-250">O código da versão do aplicativo gerenciado de Linha de Negócios (LoB) Android gerenciado.</span><span class="sxs-lookup"><span data-stu-id="4076f-250">The version code of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="4076f-251">identityVersion</span><span class="sxs-lookup"><span data-stu-id="4076f-251">identityVersion</span></span>|<span data-ttu-id="4076f-252">String</span><span class="sxs-lookup"><span data-stu-id="4076f-252">String</span></span>|<span data-ttu-id="4076f-253">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="4076f-253">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="4076f-254">Resposta</span><span class="sxs-lookup"><span data-stu-id="4076f-254">Response</span></span>
<span data-ttu-id="4076f-255">Se tiver êxito, este método retornará o código de resposta `201 Created` e o objeto [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4076f-255">If successful, this method returns a `201 Created` response code and a [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4076f-256">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4076f-256">Example</span></span>

### <a name="request"></a><span data-ttu-id="4076f-257">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4076f-257">Request</span></span>
<span data-ttu-id="4076f-258">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4076f-258">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1548

{
  "@odata.type": "#microsoft.graph.managedAndroidLobApp",
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
  "packageId": "Package Id value",
  "identityName": "Identity Name value",
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
    "v9_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="4076f-259">Resposta</span><span class="sxs-lookup"><span data-stu-id="4076f-259">Response</span></span>
<span data-ttu-id="4076f-p126">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4076f-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1720

{
  "@odata.type": "#microsoft.graph.managedAndroidLobApp",
  "id": "802b7ed3-7ed3-802b-d37e-2b80d37e2b80",
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
  "packageId": "Package Id value",
  "identityName": "Identity Name value",
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
    "v9_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```




