---
title: Atualizar windowsPhone81AppXBundle
description: Atualize as propriedades de um objeto windowsPhone81AppXBundle.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 52605849fdb65d08f3cc6a971f480ff05b922c9e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51127029"
---
# <a name="update-windowsphone81appxbundle"></a><span data-ttu-id="252f1-103">Atualizar windowsPhone81AppXBundle</span><span class="sxs-lookup"><span data-stu-id="252f1-103">Update windowsPhone81AppXBundle</span></span>

<span data-ttu-id="252f1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="252f1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="252f1-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="252f1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="252f1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="252f1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="252f1-107">Atualize as propriedades de um [objeto windowsPhone81AppXBundle.](../resources/intune-apps-windowsphone81appxbundle.md)</span><span class="sxs-lookup"><span data-stu-id="252f1-107">Update the properties of a [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="252f1-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="252f1-108">Prerequisites</span></span>
<span data-ttu-id="252f1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="252f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="252f1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="252f1-111">Permission type</span></span>|<span data-ttu-id="252f1-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="252f1-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="252f1-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="252f1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="252f1-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="252f1-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="252f1-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="252f1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="252f1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="252f1-116">Not supported.</span></span>|
|<span data-ttu-id="252f1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="252f1-117">Application</span></span>|<span data-ttu-id="252f1-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="252f1-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="252f1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="252f1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="252f1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="252f1-120">Request headers</span></span>
|<span data-ttu-id="252f1-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="252f1-121">Header</span></span>|<span data-ttu-id="252f1-122">Valor</span><span class="sxs-lookup"><span data-stu-id="252f1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="252f1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="252f1-123">Authorization</span></span>|<span data-ttu-id="252f1-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="252f1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="252f1-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="252f1-125">Accept</span></span>|<span data-ttu-id="252f1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="252f1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="252f1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="252f1-127">Request body</span></span>
<span data-ttu-id="252f1-128">No corpo da solicitação, fornece uma representação JSON para o [objeto windowsPhone81AppXBundle.](../resources/intune-apps-windowsphone81appxbundle.md)</span><span class="sxs-lookup"><span data-stu-id="252f1-128">In the request body, supply a JSON representation for the [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>

<span data-ttu-id="252f1-129">A tabela a seguir mostra as propriedades necessárias ao criar [o windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md).</span><span class="sxs-lookup"><span data-stu-id="252f1-129">The following table shows the properties that are required when you create the [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md).</span></span>

|<span data-ttu-id="252f1-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="252f1-130">Property</span></span>|<span data-ttu-id="252f1-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="252f1-131">Type</span></span>|<span data-ttu-id="252f1-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="252f1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="252f1-133">id</span><span class="sxs-lookup"><span data-stu-id="252f1-133">id</span></span>|<span data-ttu-id="252f1-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="252f1-134">String</span></span>|<span data-ttu-id="252f1-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="252f1-135">Key of the entity.</span></span> <span data-ttu-id="252f1-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="252f1-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="252f1-137">displayName</span><span class="sxs-lookup"><span data-stu-id="252f1-137">displayName</span></span>|<span data-ttu-id="252f1-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="252f1-138">String</span></span>|<span data-ttu-id="252f1-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="252f1-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="252f1-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="252f1-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="252f1-141">descrição</span><span class="sxs-lookup"><span data-stu-id="252f1-141">description</span></span>|<span data-ttu-id="252f1-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="252f1-142">String</span></span>|<span data-ttu-id="252f1-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="252f1-143">The description of the app.</span></span> <span data-ttu-id="252f1-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="252f1-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="252f1-145">publicador</span><span class="sxs-lookup"><span data-stu-id="252f1-145">publisher</span></span>|<span data-ttu-id="252f1-146">String</span><span class="sxs-lookup"><span data-stu-id="252f1-146">String</span></span>|<span data-ttu-id="252f1-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="252f1-147">The publisher of the app.</span></span> <span data-ttu-id="252f1-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="252f1-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="252f1-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="252f1-149">largeIcon</span></span>|[<span data-ttu-id="252f1-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="252f1-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="252f1-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="252f1-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="252f1-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="252f1-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="252f1-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="252f1-153">createdDateTime</span></span>|<span data-ttu-id="252f1-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="252f1-154">DateTimeOffset</span></span>|<span data-ttu-id="252f1-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="252f1-155">The date and time the app was created.</span></span> <span data-ttu-id="252f1-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="252f1-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="252f1-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="252f1-157">lastModifiedDateTime</span></span>|<span data-ttu-id="252f1-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="252f1-158">DateTimeOffset</span></span>|<span data-ttu-id="252f1-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="252f1-159">The date and time the app was last modified.</span></span> <span data-ttu-id="252f1-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="252f1-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="252f1-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="252f1-161">isFeatured</span></span>|<span data-ttu-id="252f1-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="252f1-162">Boolean</span></span>|<span data-ttu-id="252f1-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="252f1-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="252f1-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="252f1-164">privacyInformationUrl</span></span>|<span data-ttu-id="252f1-165">String</span><span class="sxs-lookup"><span data-stu-id="252f1-165">String</span></span>|<span data-ttu-id="252f1-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="252f1-166">The privacy statement Url.</span></span> <span data-ttu-id="252f1-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="252f1-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="252f1-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="252f1-168">informationUrl</span></span>|<span data-ttu-id="252f1-169">String</span><span class="sxs-lookup"><span data-stu-id="252f1-169">String</span></span>|<span data-ttu-id="252f1-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="252f1-170">The more information Url.</span></span> <span data-ttu-id="252f1-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="252f1-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="252f1-172">owner</span><span class="sxs-lookup"><span data-stu-id="252f1-172">owner</span></span>|<span data-ttu-id="252f1-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="252f1-173">String</span></span>|<span data-ttu-id="252f1-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="252f1-174">The owner of the app.</span></span> <span data-ttu-id="252f1-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="252f1-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="252f1-176">developer</span><span class="sxs-lookup"><span data-stu-id="252f1-176">developer</span></span>|<span data-ttu-id="252f1-177">String</span><span class="sxs-lookup"><span data-stu-id="252f1-177">String</span></span>|<span data-ttu-id="252f1-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="252f1-178">The developer of the app.</span></span> <span data-ttu-id="252f1-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="252f1-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="252f1-180">notes</span><span class="sxs-lookup"><span data-stu-id="252f1-180">notes</span></span>|<span data-ttu-id="252f1-181">String</span><span class="sxs-lookup"><span data-stu-id="252f1-181">String</span></span>|<span data-ttu-id="252f1-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="252f1-182">Notes for the app.</span></span> <span data-ttu-id="252f1-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="252f1-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="252f1-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="252f1-184">uploadState</span></span>|<span data-ttu-id="252f1-185">Int32</span><span class="sxs-lookup"><span data-stu-id="252f1-185">Int32</span></span>|<span data-ttu-id="252f1-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="252f1-186">The upload state.</span></span> <span data-ttu-id="252f1-187">Os valores possíveis são: 0 - `Not Ready` , 1 - `Ready` , 2 - `Processing` .</span><span class="sxs-lookup"><span data-stu-id="252f1-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="252f1-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="252f1-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="252f1-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="252f1-189">publishingState</span></span>|[<span data-ttu-id="252f1-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="252f1-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="252f1-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="252f1-191">The publishing state for the app.</span></span> <span data-ttu-id="252f1-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="252f1-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="252f1-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="252f1-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="252f1-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="252f1-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="252f1-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="252f1-195">isAssigned</span></span>|<span data-ttu-id="252f1-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="252f1-196">Boolean</span></span>|<span data-ttu-id="252f1-197">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="252f1-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="252f1-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="252f1-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="252f1-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="252f1-199">roleScopeTagIds</span></span>|<span data-ttu-id="252f1-200">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="252f1-200">String collection</span></span>|<span data-ttu-id="252f1-201">Lista de ids de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="252f1-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="252f1-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="252f1-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="252f1-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="252f1-203">dependentAppCount</span></span>|<span data-ttu-id="252f1-204">Int32</span><span class="sxs-lookup"><span data-stu-id="252f1-204">Int32</span></span>|<span data-ttu-id="252f1-205">O número total de dependências que o aplicativo filho tem.</span><span class="sxs-lookup"><span data-stu-id="252f1-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="252f1-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="252f1-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="252f1-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="252f1-207">supersedingAppCount</span></span>|<span data-ttu-id="252f1-208">Int32</span><span class="sxs-lookup"><span data-stu-id="252f1-208">Int32</span></span>|<span data-ttu-id="252f1-209">O número total de aplicativos que esse aplicativo sobressede direta ou indiretamente.</span><span class="sxs-lookup"><span data-stu-id="252f1-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="252f1-210">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="252f1-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="252f1-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="252f1-211">supersededAppCount</span></span>|<span data-ttu-id="252f1-212">Int32</span><span class="sxs-lookup"><span data-stu-id="252f1-212">Int32</span></span>|<span data-ttu-id="252f1-213">O número total de aplicativos pelos quais esse aplicativo é, direta ou indiretamente, é suplido.</span><span class="sxs-lookup"><span data-stu-id="252f1-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="252f1-214">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="252f1-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="252f1-215">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="252f1-215">committedContentVersion</span></span>|<span data-ttu-id="252f1-216">String</span><span class="sxs-lookup"><span data-stu-id="252f1-216">String</span></span>|<span data-ttu-id="252f1-217">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="252f1-217">The internal committed content version.</span></span> <span data-ttu-id="252f1-218">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="252f1-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="252f1-219">fileName</span><span class="sxs-lookup"><span data-stu-id="252f1-219">fileName</span></span>|<span data-ttu-id="252f1-220">String</span><span class="sxs-lookup"><span data-stu-id="252f1-220">String</span></span>|<span data-ttu-id="252f1-221">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="252f1-221">The name of the main Lob application file.</span></span> <span data-ttu-id="252f1-222">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="252f1-222">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="252f1-223">size</span><span class="sxs-lookup"><span data-stu-id="252f1-223">size</span></span>|<span data-ttu-id="252f1-224">Int64</span><span class="sxs-lookup"><span data-stu-id="252f1-224">Int64</span></span>|<span data-ttu-id="252f1-225">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="252f1-225">The total size, including all uploaded files.</span></span> <span data-ttu-id="252f1-226">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="252f1-226">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="252f1-227">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="252f1-227">applicableArchitectures</span></span>|[<span data-ttu-id="252f1-228">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="252f1-228">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="252f1-229">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="252f1-229">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="252f1-230">Herdado do [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span><span class="sxs-lookup"><span data-stu-id="252f1-230">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span></span> <span data-ttu-id="252f1-231">Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="252f1-231">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="252f1-232">identityName</span><span class="sxs-lookup"><span data-stu-id="252f1-232">identityName</span></span>|<span data-ttu-id="252f1-233">String</span><span class="sxs-lookup"><span data-stu-id="252f1-233">String</span></span>|<span data-ttu-id="252f1-234">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="252f1-234">The Identity Name.</span></span> <span data-ttu-id="252f1-235">Herdado do [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="252f1-235">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="252f1-236">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="252f1-236">identityPublisherHash</span></span>|<span data-ttu-id="252f1-237">String</span><span class="sxs-lookup"><span data-stu-id="252f1-237">String</span></span>|<span data-ttu-id="252f1-238">O Hash do Publicador de Identidade.</span><span class="sxs-lookup"><span data-stu-id="252f1-238">The Identity Publisher Hash.</span></span> <span data-ttu-id="252f1-239">Herdado do [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="252f1-239">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="252f1-240">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="252f1-240">identityResourceIdentifier</span></span>|<span data-ttu-id="252f1-241">String</span><span class="sxs-lookup"><span data-stu-id="252f1-241">String</span></span>|<span data-ttu-id="252f1-242">O Identificador de Recurso da Identidade.</span><span class="sxs-lookup"><span data-stu-id="252f1-242">The Identity Resource Identifier.</span></span> <span data-ttu-id="252f1-243">Herdado do [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="252f1-243">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="252f1-244">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="252f1-244">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="252f1-245">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="252f1-245">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="252f1-246">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="252f1-246">The value for the minimum applicable operating system.</span></span> <span data-ttu-id="252f1-247">Herdado do [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="252f1-247">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="252f1-248">phoneProductIdentifier</span><span class="sxs-lookup"><span data-stu-id="252f1-248">phoneProductIdentifier</span></span>|<span data-ttu-id="252f1-249">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="252f1-249">String</span></span>|<span data-ttu-id="252f1-250">O Identificador de Produto de Telefone.</span><span class="sxs-lookup"><span data-stu-id="252f1-250">The Phone Product Identifier.</span></span> <span data-ttu-id="252f1-251">Herdado do [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="252f1-251">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="252f1-252">phonePublisherId</span><span class="sxs-lookup"><span data-stu-id="252f1-252">phonePublisherId</span></span>|<span data-ttu-id="252f1-253">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="252f1-253">String</span></span>|<span data-ttu-id="252f1-254">A ID do Editor de Telefones. Herdada do [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="252f1-254">The Phone Publisher Id. Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="252f1-255">identityVersion</span><span class="sxs-lookup"><span data-stu-id="252f1-255">identityVersion</span></span>|<span data-ttu-id="252f1-256">String</span><span class="sxs-lookup"><span data-stu-id="252f1-256">String</span></span>|<span data-ttu-id="252f1-257">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="252f1-257">The identity version.</span></span> <span data-ttu-id="252f1-258">Herdado do [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="252f1-258">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="252f1-259">appXPackageInformationList</span><span class="sxs-lookup"><span data-stu-id="252f1-259">appXPackageInformationList</span></span>|<span data-ttu-id="252f1-260">[Coleção windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md)</span><span class="sxs-lookup"><span data-stu-id="252f1-260">[windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md) collection</span></span>|<span data-ttu-id="252f1-261">A lista de Informações do Pacote AppX.</span><span class="sxs-lookup"><span data-stu-id="252f1-261">The list of AppX Package Information.</span></span>|



## <a name="response"></a><span data-ttu-id="252f1-262">Resposta</span><span class="sxs-lookup"><span data-stu-id="252f1-262">Response</span></span>
<span data-ttu-id="252f1-263">Se tiver êxito, este método retornará um código de resposta e um objeto `200 OK` [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="252f1-263">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="252f1-264">Exemplo</span><span class="sxs-lookup"><span data-stu-id="252f1-264">Example</span></span>

### <a name="request"></a><span data-ttu-id="252f1-265">Solicitação</span><span class="sxs-lookup"><span data-stu-id="252f1-265">Request</span></span>
<span data-ttu-id="252f1-266">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="252f1-266">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 2468

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
    "v10_1903": true,
    "v10_1909": true,
    "v10_2004": true
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
        "v10_1903": true,
        "v10_1909": true,
        "v10_2004": true
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="252f1-267">Resposta</span><span class="sxs-lookup"><span data-stu-id="252f1-267">Response</span></span>
<span data-ttu-id="252f1-p131">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="252f1-p131">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2640

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
    "v10_1903": true,
    "v10_1909": true,
    "v10_2004": true
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
        "v10_1903": true,
        "v10_1909": true,
        "v10_2004": true
      }
    }
  ]
}
```




