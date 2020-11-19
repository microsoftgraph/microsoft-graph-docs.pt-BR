---
title: Atualizar windowsPhone81AppXBundle
description: Atualiza as propriedades de um objeto windowsPhone81AppXBundle.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 11e0141ed1884006642cb9bb054dd2347582e459
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49246632"
---
# <a name="update-windowsphone81appxbundle"></a><span data-ttu-id="4b277-103">Atualizar windowsPhone81AppXBundle</span><span class="sxs-lookup"><span data-stu-id="4b277-103">Update windowsPhone81AppXBundle</span></span>

<span data-ttu-id="4b277-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b277-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4b277-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4b277-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4b277-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4b277-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b277-107">Atualiza as propriedades de um objeto [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) .</span><span class="sxs-lookup"><span data-stu-id="4b277-107">Update the properties of a [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4b277-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4b277-108">Prerequisites</span></span>
<span data-ttu-id="4b277-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b277-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b277-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4b277-111">Permission type</span></span>|<span data-ttu-id="4b277-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4b277-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b277-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4b277-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4b277-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b277-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4b277-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4b277-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b277-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4b277-116">Not supported.</span></span>|
|<span data-ttu-id="4b277-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4b277-117">Application</span></span>|<span data-ttu-id="4b277-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b277-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b277-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4b277-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="4b277-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4b277-120">Request headers</span></span>
|<span data-ttu-id="4b277-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4b277-121">Header</span></span>|<span data-ttu-id="4b277-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4b277-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b277-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4b277-123">Authorization</span></span>|<span data-ttu-id="4b277-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4b277-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b277-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4b277-125">Accept</span></span>|<span data-ttu-id="4b277-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4b277-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b277-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4b277-127">Request body</span></span>
<span data-ttu-id="4b277-128">No corpo da solicitação, forneça uma representação JSON do objeto [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) .</span><span class="sxs-lookup"><span data-stu-id="4b277-128">In the request body, supply a JSON representation for the [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>

<span data-ttu-id="4b277-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md).</span><span class="sxs-lookup"><span data-stu-id="4b277-129">The following table shows the properties that are required when you create the [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md).</span></span>

|<span data-ttu-id="4b277-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4b277-130">Property</span></span>|<span data-ttu-id="4b277-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4b277-131">Type</span></span>|<span data-ttu-id="4b277-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b277-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b277-133">id</span><span class="sxs-lookup"><span data-stu-id="4b277-133">id</span></span>|<span data-ttu-id="4b277-134">String</span><span class="sxs-lookup"><span data-stu-id="4b277-134">String</span></span>|<span data-ttu-id="4b277-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4b277-135">Key of the entity.</span></span> <span data-ttu-id="4b277-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4b277-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4b277-137">displayName</span><span class="sxs-lookup"><span data-stu-id="4b277-137">displayName</span></span>|<span data-ttu-id="4b277-138">String</span><span class="sxs-lookup"><span data-stu-id="4b277-138">String</span></span>|<span data-ttu-id="4b277-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="4b277-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="4b277-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4b277-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4b277-141">description</span><span class="sxs-lookup"><span data-stu-id="4b277-141">description</span></span>|<span data-ttu-id="4b277-142">String</span><span class="sxs-lookup"><span data-stu-id="4b277-142">String</span></span>|<span data-ttu-id="4b277-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4b277-143">The description of the app.</span></span> <span data-ttu-id="4b277-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4b277-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4b277-145">publicador</span><span class="sxs-lookup"><span data-stu-id="4b277-145">publisher</span></span>|<span data-ttu-id="4b277-146">String</span><span class="sxs-lookup"><span data-stu-id="4b277-146">String</span></span>|<span data-ttu-id="4b277-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4b277-147">The publisher of the app.</span></span> <span data-ttu-id="4b277-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4b277-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4b277-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="4b277-149">largeIcon</span></span>|[<span data-ttu-id="4b277-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="4b277-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="4b277-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="4b277-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="4b277-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4b277-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4b277-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4b277-153">createdDateTime</span></span>|<span data-ttu-id="4b277-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b277-154">DateTimeOffset</span></span>|<span data-ttu-id="4b277-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4b277-155">The date and time the app was created.</span></span> <span data-ttu-id="4b277-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4b277-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4b277-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4b277-157">lastModifiedDateTime</span></span>|<span data-ttu-id="4b277-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b277-158">DateTimeOffset</span></span>|<span data-ttu-id="4b277-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="4b277-159">The date and time the app was last modified.</span></span> <span data-ttu-id="4b277-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4b277-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4b277-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="4b277-161">isFeatured</span></span>|<span data-ttu-id="4b277-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b277-162">Boolean</span></span>|<span data-ttu-id="4b277-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4b277-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4b277-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="4b277-164">privacyInformationUrl</span></span>|<span data-ttu-id="4b277-165">String</span><span class="sxs-lookup"><span data-stu-id="4b277-165">String</span></span>|<span data-ttu-id="4b277-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="4b277-166">The privacy statement Url.</span></span> <span data-ttu-id="4b277-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4b277-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4b277-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="4b277-168">informationUrl</span></span>|<span data-ttu-id="4b277-169">String</span><span class="sxs-lookup"><span data-stu-id="4b277-169">String</span></span>|<span data-ttu-id="4b277-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="4b277-170">The more information Url.</span></span> <span data-ttu-id="4b277-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4b277-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4b277-172">owner</span><span class="sxs-lookup"><span data-stu-id="4b277-172">owner</span></span>|<span data-ttu-id="4b277-173">String</span><span class="sxs-lookup"><span data-stu-id="4b277-173">String</span></span>|<span data-ttu-id="4b277-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="4b277-174">The owner of the app.</span></span> <span data-ttu-id="4b277-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4b277-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4b277-176">developer</span><span class="sxs-lookup"><span data-stu-id="4b277-176">developer</span></span>|<span data-ttu-id="4b277-177">String</span><span class="sxs-lookup"><span data-stu-id="4b277-177">String</span></span>|<span data-ttu-id="4b277-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4b277-178">The developer of the app.</span></span> <span data-ttu-id="4b277-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4b277-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4b277-180">notes</span><span class="sxs-lookup"><span data-stu-id="4b277-180">notes</span></span>|<span data-ttu-id="4b277-181">String</span><span class="sxs-lookup"><span data-stu-id="4b277-181">String</span></span>|<span data-ttu-id="4b277-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4b277-182">Notes for the app.</span></span> <span data-ttu-id="4b277-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4b277-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4b277-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="4b277-184">uploadState</span></span>|<span data-ttu-id="4b277-185">Int32</span><span class="sxs-lookup"><span data-stu-id="4b277-185">Int32</span></span>|<span data-ttu-id="4b277-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="4b277-186">The upload state.</span></span> <span data-ttu-id="4b277-187">Os valores possíveis são: 0- `Not Ready` , 1- `Ready` , 2- `Processing` .</span><span class="sxs-lookup"><span data-stu-id="4b277-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="4b277-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4b277-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4b277-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="4b277-189">publishingState</span></span>|[<span data-ttu-id="4b277-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="4b277-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="4b277-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4b277-191">The publishing state for the app.</span></span> <span data-ttu-id="4b277-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="4b277-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="4b277-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4b277-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="4b277-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="4b277-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="4b277-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="4b277-195">isAssigned</span></span>|<span data-ttu-id="4b277-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b277-196">Boolean</span></span>|<span data-ttu-id="4b277-197">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="4b277-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="4b277-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4b277-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4b277-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4b277-199">roleScopeTagIds</span></span>|<span data-ttu-id="4b277-200">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="4b277-200">String collection</span></span>|<span data-ttu-id="4b277-201">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="4b277-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="4b277-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4b277-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4b277-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="4b277-203">dependentAppCount</span></span>|<span data-ttu-id="4b277-204">Int32</span><span class="sxs-lookup"><span data-stu-id="4b277-204">Int32</span></span>|<span data-ttu-id="4b277-205">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="4b277-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="4b277-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4b277-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4b277-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="4b277-207">supersedingAppCount</span></span>|<span data-ttu-id="4b277-208">Int32</span><span class="sxs-lookup"><span data-stu-id="4b277-208">Int32</span></span>|<span data-ttu-id="4b277-209">O número total de aplicativos que este aplicativo substitui direta ou indiretamente.</span><span class="sxs-lookup"><span data-stu-id="4b277-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="4b277-210">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4b277-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4b277-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="4b277-211">supersededAppCount</span></span>|<span data-ttu-id="4b277-212">Int32</span><span class="sxs-lookup"><span data-stu-id="4b277-212">Int32</span></span>|<span data-ttu-id="4b277-213">O número total de aplicativos que este aplicativo está substituindo direta ou indiretamente por.</span><span class="sxs-lookup"><span data-stu-id="4b277-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="4b277-214">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4b277-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4b277-215">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="4b277-215">committedContentVersion</span></span>|<span data-ttu-id="4b277-216">String</span><span class="sxs-lookup"><span data-stu-id="4b277-216">String</span></span>|<span data-ttu-id="4b277-217">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="4b277-217">The internal committed content version.</span></span> <span data-ttu-id="4b277-218">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="4b277-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="4b277-219">fileName</span><span class="sxs-lookup"><span data-stu-id="4b277-219">fileName</span></span>|<span data-ttu-id="4b277-220">String</span><span class="sxs-lookup"><span data-stu-id="4b277-220">String</span></span>|<span data-ttu-id="4b277-221">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="4b277-221">The name of the main Lob application file.</span></span> <span data-ttu-id="4b277-222">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="4b277-222">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="4b277-223">size</span><span class="sxs-lookup"><span data-stu-id="4b277-223">size</span></span>|<span data-ttu-id="4b277-224">Int64</span><span class="sxs-lookup"><span data-stu-id="4b277-224">Int64</span></span>|<span data-ttu-id="4b277-225">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="4b277-225">The total size, including all uploaded files.</span></span> <span data-ttu-id="4b277-226">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="4b277-226">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="4b277-227">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="4b277-227">applicableArchitectures</span></span>|[<span data-ttu-id="4b277-228">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="4b277-228">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="4b277-229">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="4b277-229">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="4b277-230">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span><span class="sxs-lookup"><span data-stu-id="4b277-230">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span></span> <span data-ttu-id="4b277-231">Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="4b277-231">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="4b277-232">identityName</span><span class="sxs-lookup"><span data-stu-id="4b277-232">identityName</span></span>|<span data-ttu-id="4b277-233">String</span><span class="sxs-lookup"><span data-stu-id="4b277-233">String</span></span>|<span data-ttu-id="4b277-234">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="4b277-234">The Identity Name.</span></span> <span data-ttu-id="4b277-235">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="4b277-235">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="4b277-236">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="4b277-236">identityPublisherHash</span></span>|<span data-ttu-id="4b277-237">String</span><span class="sxs-lookup"><span data-stu-id="4b277-237">String</span></span>|<span data-ttu-id="4b277-238">O Hash do Publicador de Identidade.</span><span class="sxs-lookup"><span data-stu-id="4b277-238">The Identity Publisher Hash.</span></span> <span data-ttu-id="4b277-239">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="4b277-239">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="4b277-240">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="4b277-240">identityResourceIdentifier</span></span>|<span data-ttu-id="4b277-241">String</span><span class="sxs-lookup"><span data-stu-id="4b277-241">String</span></span>|<span data-ttu-id="4b277-242">O Identificador de Recurso da Identidade.</span><span class="sxs-lookup"><span data-stu-id="4b277-242">The Identity Resource Identifier.</span></span> <span data-ttu-id="4b277-243">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="4b277-243">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="4b277-244">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="4b277-244">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="4b277-245">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="4b277-245">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="4b277-246">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="4b277-246">The value for the minimum applicable operating system.</span></span> <span data-ttu-id="4b277-247">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="4b277-247">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="4b277-248">phoneProductIdentifier</span><span class="sxs-lookup"><span data-stu-id="4b277-248">phoneProductIdentifier</span></span>|<span data-ttu-id="4b277-249">String</span><span class="sxs-lookup"><span data-stu-id="4b277-249">String</span></span>|<span data-ttu-id="4b277-250">O identificador do produto de telefone.</span><span class="sxs-lookup"><span data-stu-id="4b277-250">The Phone Product Identifier.</span></span> <span data-ttu-id="4b277-251">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="4b277-251">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="4b277-252">phonePublisherId</span><span class="sxs-lookup"><span data-stu-id="4b277-252">phonePublisherId</span></span>|<span data-ttu-id="4b277-253">String</span><span class="sxs-lookup"><span data-stu-id="4b277-253">String</span></span>|<span data-ttu-id="4b277-254">A ID do editor do telefone. herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="4b277-254">The Phone Publisher Id. Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="4b277-255">identityVersion</span><span class="sxs-lookup"><span data-stu-id="4b277-255">identityVersion</span></span>|<span data-ttu-id="4b277-256">String</span><span class="sxs-lookup"><span data-stu-id="4b277-256">String</span></span>|<span data-ttu-id="4b277-257">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="4b277-257">The identity version.</span></span> <span data-ttu-id="4b277-258">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="4b277-258">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="4b277-259">appXPackageInformationList</span><span class="sxs-lookup"><span data-stu-id="4b277-259">appXPackageInformationList</span></span>|<span data-ttu-id="4b277-260">coleção [windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md)</span><span class="sxs-lookup"><span data-stu-id="4b277-260">[windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md) collection</span></span>|<span data-ttu-id="4b277-261">A lista de informações do pacote AppX.</span><span class="sxs-lookup"><span data-stu-id="4b277-261">The list of AppX Package Information.</span></span>|



## <a name="response"></a><span data-ttu-id="4b277-262">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b277-262">Response</span></span>
<span data-ttu-id="4b277-263">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4b277-263">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b277-264">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4b277-264">Example</span></span>

### <a name="request"></a><span data-ttu-id="4b277-265">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4b277-265">Request</span></span>
<span data-ttu-id="4b277-266">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4b277-266">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 2368

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppXBundle",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "applicableArchitectures": "x86",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true,
    "v10_1809": true,
    "v10_1903": true
  },
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value",
  "appXPackageInformationList": [
    {
      "@odata.type": "microsoft.graph.windowsPackageInformation",
      "applicableArchitecture": "x86",
      "displayName": "Display Name value",
      "identityName": "Identity Name value",
      "identityPublisher": "Identity Publisher value",
      "identityResourceIdentifier": "Identity Resource Identifier value",
      "identityVersion": "Identity Version value",
      "minimumSupportedOperatingSystem": {
        "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
        "v8_0": true,
        "v8_1": true,
        "v10_0": true,
        "v10_1607": true,
        "v10_1703": true,
        "v10_1709": true,
        "v10_1803": true,
        "v10_1809": true,
        "v10_1903": true
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="4b277-267">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b277-267">Response</span></span>
<span data-ttu-id="4b277-p131">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4b277-p131">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2540

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppXBundle",
  "id": "2433be7c-be7c-2433-7cbe-33247cbe3324",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "applicableArchitectures": "x86",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true,
    "v10_1809": true,
    "v10_1903": true
  },
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value",
  "appXPackageInformationList": [
    {
      "@odata.type": "microsoft.graph.windowsPackageInformation",
      "applicableArchitecture": "x86",
      "displayName": "Display Name value",
      "identityName": "Identity Name value",
      "identityPublisher": "Identity Publisher value",
      "identityResourceIdentifier": "Identity Resource Identifier value",
      "identityVersion": "Identity Version value",
      "minimumSupportedOperatingSystem": {
        "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
        "v8_0": true,
        "v8_1": true,
        "v10_0": true,
        "v10_1607": true,
        "v10_1703": true,
        "v10_1709": true,
        "v10_1803": true,
        "v10_1809": true,
        "v10_1903": true
      }
    }
  ]
}
```




