---
title: Atualizar windowsPhone81AppX
description: Atualize as propriedades de um objeto windowsPhone81AppX.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 92d576a87f8440cb263900dd57b664a358393ee4
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51862936"
---
# <a name="update-windowsphone81appx"></a><span data-ttu-id="f2cfe-103">Atualizar windowsPhone81AppX</span><span class="sxs-lookup"><span data-stu-id="f2cfe-103">Update windowsPhone81AppX</span></span>

<span data-ttu-id="f2cfe-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2cfe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f2cfe-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f2cfe-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f2cfe-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f2cfe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2cfe-107">Atualize as propriedades de um [objeto windowsPhone81AppX.](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="f2cfe-107">Update the properties of a [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f2cfe-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f2cfe-108">Prerequisites</span></span>
<span data-ttu-id="f2cfe-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2cfe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2cfe-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f2cfe-111">Permission type</span></span>|<span data-ttu-id="f2cfe-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f2cfe-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2cfe-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f2cfe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f2cfe-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2cfe-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f2cfe-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f2cfe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2cfe-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f2cfe-116">Not supported.</span></span>|
|<span data-ttu-id="f2cfe-117">Application</span><span class="sxs-lookup"><span data-stu-id="f2cfe-117">Application</span></span>|<span data-ttu-id="f2cfe-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2cfe-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2cfe-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f2cfe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="f2cfe-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f2cfe-120">Request headers</span></span>
|<span data-ttu-id="f2cfe-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f2cfe-121">Header</span></span>|<span data-ttu-id="f2cfe-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f2cfe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f2cfe-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f2cfe-123">Authorization</span></span>|<span data-ttu-id="f2cfe-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f2cfe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f2cfe-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f2cfe-125">Accept</span></span>|<span data-ttu-id="f2cfe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f2cfe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2cfe-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f2cfe-127">Request body</span></span>
<span data-ttu-id="f2cfe-128">No corpo da solicitação, fornece uma representação JSON para o [objeto windowsPhone81AppX.](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="f2cfe-128">In the request body, supply a JSON representation for the [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object.</span></span>

<span data-ttu-id="f2cfe-129">A tabela a seguir mostra as propriedades necessárias ao criar [o windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span><span class="sxs-lookup"><span data-stu-id="f2cfe-129">The following table shows the properties that are required when you create the [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span></span>

|<span data-ttu-id="f2cfe-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f2cfe-130">Property</span></span>|<span data-ttu-id="f2cfe-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2cfe-131">Type</span></span>|<span data-ttu-id="f2cfe-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2cfe-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2cfe-133">id</span><span class="sxs-lookup"><span data-stu-id="f2cfe-133">id</span></span>|<span data-ttu-id="f2cfe-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2cfe-134">String</span></span>|<span data-ttu-id="f2cfe-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f2cfe-135">Key of the entity.</span></span> <span data-ttu-id="f2cfe-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2cfe-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2cfe-137">displayName</span><span class="sxs-lookup"><span data-stu-id="f2cfe-137">displayName</span></span>|<span data-ttu-id="f2cfe-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2cfe-138">String</span></span>|<span data-ttu-id="f2cfe-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="f2cfe-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="f2cfe-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2cfe-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2cfe-141">description</span><span class="sxs-lookup"><span data-stu-id="f2cfe-141">description</span></span>|<span data-ttu-id="f2cfe-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2cfe-142">String</span></span>|<span data-ttu-id="f2cfe-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f2cfe-143">The description of the app.</span></span> <span data-ttu-id="f2cfe-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2cfe-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2cfe-145">publicador</span><span class="sxs-lookup"><span data-stu-id="f2cfe-145">publisher</span></span>|<span data-ttu-id="f2cfe-146">String</span><span class="sxs-lookup"><span data-stu-id="f2cfe-146">String</span></span>|<span data-ttu-id="f2cfe-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f2cfe-147">The publisher of the app.</span></span> <span data-ttu-id="f2cfe-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2cfe-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2cfe-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="f2cfe-149">largeIcon</span></span>|[<span data-ttu-id="f2cfe-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f2cfe-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f2cfe-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="f2cfe-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="f2cfe-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2cfe-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2cfe-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f2cfe-153">createdDateTime</span></span>|<span data-ttu-id="f2cfe-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2cfe-154">DateTimeOffset</span></span>|<span data-ttu-id="f2cfe-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f2cfe-155">The date and time the app was created.</span></span> <span data-ttu-id="f2cfe-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2cfe-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2cfe-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f2cfe-157">lastModifiedDateTime</span></span>|<span data-ttu-id="f2cfe-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2cfe-158">DateTimeOffset</span></span>|<span data-ttu-id="f2cfe-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="f2cfe-159">The date and time the app was last modified.</span></span> <span data-ttu-id="f2cfe-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2cfe-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2cfe-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="f2cfe-161">isFeatured</span></span>|<span data-ttu-id="f2cfe-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="f2cfe-162">Boolean</span></span>|<span data-ttu-id="f2cfe-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2cfe-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2cfe-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f2cfe-164">privacyInformationUrl</span></span>|<span data-ttu-id="f2cfe-165">String</span><span class="sxs-lookup"><span data-stu-id="f2cfe-165">String</span></span>|<span data-ttu-id="f2cfe-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="f2cfe-166">The privacy statement Url.</span></span> <span data-ttu-id="f2cfe-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2cfe-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2cfe-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f2cfe-168">informationUrl</span></span>|<span data-ttu-id="f2cfe-169">String</span><span class="sxs-lookup"><span data-stu-id="f2cfe-169">String</span></span>|<span data-ttu-id="f2cfe-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="f2cfe-170">The more information Url.</span></span> <span data-ttu-id="f2cfe-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2cfe-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2cfe-172">owner</span><span class="sxs-lookup"><span data-stu-id="f2cfe-172">owner</span></span>|<span data-ttu-id="f2cfe-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2cfe-173">String</span></span>|<span data-ttu-id="f2cfe-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="f2cfe-174">The owner of the app.</span></span> <span data-ttu-id="f2cfe-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2cfe-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2cfe-176">developer</span><span class="sxs-lookup"><span data-stu-id="f2cfe-176">developer</span></span>|<span data-ttu-id="f2cfe-177">String</span><span class="sxs-lookup"><span data-stu-id="f2cfe-177">String</span></span>|<span data-ttu-id="f2cfe-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f2cfe-178">The developer of the app.</span></span> <span data-ttu-id="f2cfe-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2cfe-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2cfe-180">notes</span><span class="sxs-lookup"><span data-stu-id="f2cfe-180">notes</span></span>|<span data-ttu-id="f2cfe-181">String</span><span class="sxs-lookup"><span data-stu-id="f2cfe-181">String</span></span>|<span data-ttu-id="f2cfe-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f2cfe-182">Notes for the app.</span></span> <span data-ttu-id="f2cfe-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2cfe-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2cfe-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="f2cfe-184">uploadState</span></span>|<span data-ttu-id="f2cfe-185">Int32</span><span class="sxs-lookup"><span data-stu-id="f2cfe-185">Int32</span></span>|<span data-ttu-id="f2cfe-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="f2cfe-186">The upload state.</span></span> <span data-ttu-id="f2cfe-187">Os valores possíveis são: 0 - `Not Ready` , 1 - `Ready` , 2 - `Processing` .</span><span class="sxs-lookup"><span data-stu-id="f2cfe-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="f2cfe-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2cfe-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2cfe-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="f2cfe-189">publishingState</span></span>|[<span data-ttu-id="f2cfe-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="f2cfe-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="f2cfe-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f2cfe-191">The publishing state for the app.</span></span> <span data-ttu-id="f2cfe-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="f2cfe-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="f2cfe-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f2cfe-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="f2cfe-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="f2cfe-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="f2cfe-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="f2cfe-195">isAssigned</span></span>|<span data-ttu-id="f2cfe-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="f2cfe-196">Boolean</span></span>|<span data-ttu-id="f2cfe-197">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="f2cfe-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="f2cfe-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2cfe-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2cfe-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f2cfe-199">roleScopeTagIds</span></span>|<span data-ttu-id="f2cfe-200">Coleção String</span><span class="sxs-lookup"><span data-stu-id="f2cfe-200">String collection</span></span>|<span data-ttu-id="f2cfe-201">Lista de ids de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="f2cfe-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="f2cfe-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2cfe-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2cfe-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="f2cfe-203">dependentAppCount</span></span>|<span data-ttu-id="f2cfe-204">Int32</span><span class="sxs-lookup"><span data-stu-id="f2cfe-204">Int32</span></span>|<span data-ttu-id="f2cfe-205">O número total de dependências que o aplicativo filho tem.</span><span class="sxs-lookup"><span data-stu-id="f2cfe-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="f2cfe-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2cfe-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2cfe-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="f2cfe-207">supersedingAppCount</span></span>|<span data-ttu-id="f2cfe-208">Int32</span><span class="sxs-lookup"><span data-stu-id="f2cfe-208">Int32</span></span>|<span data-ttu-id="f2cfe-209">O número total de aplicativos que esse aplicativo sobressede direta ou indiretamente.</span><span class="sxs-lookup"><span data-stu-id="f2cfe-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="f2cfe-210">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2cfe-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2cfe-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="f2cfe-211">supersededAppCount</span></span>|<span data-ttu-id="f2cfe-212">Int32</span><span class="sxs-lookup"><span data-stu-id="f2cfe-212">Int32</span></span>|<span data-ttu-id="f2cfe-213">O número total de aplicativos pelos quais esse aplicativo é, direta ou indiretamente, é suplido.</span><span class="sxs-lookup"><span data-stu-id="f2cfe-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="f2cfe-214">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2cfe-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2cfe-215">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="f2cfe-215">committedContentVersion</span></span>|<span data-ttu-id="f2cfe-216">String</span><span class="sxs-lookup"><span data-stu-id="f2cfe-216">String</span></span>|<span data-ttu-id="f2cfe-217">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="f2cfe-217">The internal committed content version.</span></span> <span data-ttu-id="f2cfe-218">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2cfe-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="f2cfe-219">fileName</span><span class="sxs-lookup"><span data-stu-id="f2cfe-219">fileName</span></span>|<span data-ttu-id="f2cfe-220">String</span><span class="sxs-lookup"><span data-stu-id="f2cfe-220">String</span></span>|<span data-ttu-id="f2cfe-221">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="f2cfe-221">The name of the main Lob application file.</span></span> <span data-ttu-id="f2cfe-222">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2cfe-222">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="f2cfe-223">size</span><span class="sxs-lookup"><span data-stu-id="f2cfe-223">size</span></span>|<span data-ttu-id="f2cfe-224">Int64</span><span class="sxs-lookup"><span data-stu-id="f2cfe-224">Int64</span></span>|<span data-ttu-id="f2cfe-225">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="f2cfe-225">The total size, including all uploaded files.</span></span> <span data-ttu-id="f2cfe-226">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2cfe-226">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="f2cfe-227">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="f2cfe-227">applicableArchitectures</span></span>|[<span data-ttu-id="f2cfe-228">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="f2cfe-228">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="f2cfe-229">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="f2cfe-229">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="f2cfe-230">Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="f2cfe-230">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="f2cfe-231">identityName</span><span class="sxs-lookup"><span data-stu-id="f2cfe-231">identityName</span></span>|<span data-ttu-id="f2cfe-232">String</span><span class="sxs-lookup"><span data-stu-id="f2cfe-232">String</span></span>|<span data-ttu-id="f2cfe-233">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="f2cfe-233">The Identity Name.</span></span>|
|<span data-ttu-id="f2cfe-234">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="f2cfe-234">identityPublisherHash</span></span>|<span data-ttu-id="f2cfe-235">String</span><span class="sxs-lookup"><span data-stu-id="f2cfe-235">String</span></span>|<span data-ttu-id="f2cfe-236">O Hash do Publicador de Identidade.</span><span class="sxs-lookup"><span data-stu-id="f2cfe-236">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="f2cfe-237">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="f2cfe-237">identityResourceIdentifier</span></span>|<span data-ttu-id="f2cfe-238">String</span><span class="sxs-lookup"><span data-stu-id="f2cfe-238">String</span></span>|<span data-ttu-id="f2cfe-239">O Identificador de Recurso da Identidade.</span><span class="sxs-lookup"><span data-stu-id="f2cfe-239">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="f2cfe-240">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f2cfe-240">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="f2cfe-241">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f2cfe-241">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="f2cfe-242">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="f2cfe-242">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="f2cfe-243">phoneProductIdentifier</span><span class="sxs-lookup"><span data-stu-id="f2cfe-243">phoneProductIdentifier</span></span>|<span data-ttu-id="f2cfe-244">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="f2cfe-244">String</span></span>|<span data-ttu-id="f2cfe-245">O Identificador de Produto de Telefone.</span><span class="sxs-lookup"><span data-stu-id="f2cfe-245">The Phone Product Identifier.</span></span>|
|<span data-ttu-id="f2cfe-246">phonePublisherId</span><span class="sxs-lookup"><span data-stu-id="f2cfe-246">phonePublisherId</span></span>|<span data-ttu-id="f2cfe-247">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="f2cfe-247">String</span></span>|<span data-ttu-id="f2cfe-248">A ID do Editor de Telefones.</span><span class="sxs-lookup"><span data-stu-id="f2cfe-248">The Phone Publisher Id.</span></span>|
|<span data-ttu-id="f2cfe-249">identityVersion</span><span class="sxs-lookup"><span data-stu-id="f2cfe-249">identityVersion</span></span>|<span data-ttu-id="f2cfe-250">String</span><span class="sxs-lookup"><span data-stu-id="f2cfe-250">String</span></span>|<span data-ttu-id="f2cfe-251">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="f2cfe-251">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="f2cfe-252">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2cfe-252">Response</span></span>
<span data-ttu-id="f2cfe-253">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f2cfe-253">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2cfe-254">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f2cfe-254">Example</span></span>

### <a name="request"></a><span data-ttu-id="f2cfe-255">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f2cfe-255">Request</span></span>
<span data-ttu-id="f2cfe-256">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f2cfe-256">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1639

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppX",
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
    "v10_2004": true,
    "v10_2H20": true
  },
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="f2cfe-257">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2cfe-257">Response</span></span>
<span data-ttu-id="f2cfe-p125">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f2cfe-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1811

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppX",
  "id": "4ff27f80-7f80-4ff2-807f-f24f807ff24f",
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
    "v10_2004": true,
    "v10_2H20": true
  },
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value"
}
```




