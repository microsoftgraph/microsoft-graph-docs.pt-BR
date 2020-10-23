---
title: Criar windowsPhone81AppXBundle
description: Criar um novo objeto windowsPhone81AppXBundle.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 519469de33158ae2199b3a31b64f09fbd046eed2
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48697137"
---
# <a name="create-windowsphone81appxbundle"></a><span data-ttu-id="ec72b-103">Criar windowsPhone81AppXBundle</span><span class="sxs-lookup"><span data-stu-id="ec72b-103">Create windowsPhone81AppXBundle</span></span>

<span data-ttu-id="ec72b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec72b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ec72b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ec72b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ec72b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ec72b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec72b-107">Criar um novo objeto [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) .</span><span class="sxs-lookup"><span data-stu-id="ec72b-107">Create a new [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ec72b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ec72b-108">Prerequisites</span></span>
<span data-ttu-id="ec72b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec72b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec72b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ec72b-111">Permission type</span></span>|<span data-ttu-id="ec72b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ec72b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ec72b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ec72b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ec72b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec72b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ec72b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ec72b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ec72b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ec72b-116">Not supported.</span></span>|
|<span data-ttu-id="ec72b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ec72b-117">Application</span></span>|<span data-ttu-id="ec72b-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec72b-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ec72b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ec72b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="ec72b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ec72b-120">Request headers</span></span>
|<span data-ttu-id="ec72b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ec72b-121">Header</span></span>|<span data-ttu-id="ec72b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ec72b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ec72b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ec72b-123">Authorization</span></span>|<span data-ttu-id="ec72b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ec72b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ec72b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ec72b-125">Accept</span></span>|<span data-ttu-id="ec72b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ec72b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec72b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ec72b-127">Request body</span></span>
<span data-ttu-id="ec72b-128">No corpo da solicitação, forneça uma representação JSON do objeto windowsPhone81AppXBundle.</span><span class="sxs-lookup"><span data-stu-id="ec72b-128">In the request body, supply a JSON representation for the windowsPhone81AppXBundle object.</span></span>

<span data-ttu-id="ec72b-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsPhone81AppXBundle.</span><span class="sxs-lookup"><span data-stu-id="ec72b-129">The following table shows the properties that are required when you create the windowsPhone81AppXBundle.</span></span>

|<span data-ttu-id="ec72b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ec72b-130">Property</span></span>|<span data-ttu-id="ec72b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ec72b-131">Type</span></span>|<span data-ttu-id="ec72b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec72b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec72b-133">id</span><span class="sxs-lookup"><span data-stu-id="ec72b-133">id</span></span>|<span data-ttu-id="ec72b-134">String</span><span class="sxs-lookup"><span data-stu-id="ec72b-134">String</span></span>|<span data-ttu-id="ec72b-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ec72b-135">Key of the entity.</span></span> <span data-ttu-id="ec72b-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ec72b-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ec72b-137">displayName</span><span class="sxs-lookup"><span data-stu-id="ec72b-137">displayName</span></span>|<span data-ttu-id="ec72b-138">String</span><span class="sxs-lookup"><span data-stu-id="ec72b-138">String</span></span>|<span data-ttu-id="ec72b-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="ec72b-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="ec72b-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ec72b-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ec72b-141">description</span><span class="sxs-lookup"><span data-stu-id="ec72b-141">description</span></span>|<span data-ttu-id="ec72b-142">String</span><span class="sxs-lookup"><span data-stu-id="ec72b-142">String</span></span>|<span data-ttu-id="ec72b-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ec72b-143">The description of the app.</span></span> <span data-ttu-id="ec72b-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ec72b-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ec72b-145">publicador</span><span class="sxs-lookup"><span data-stu-id="ec72b-145">publisher</span></span>|<span data-ttu-id="ec72b-146">String</span><span class="sxs-lookup"><span data-stu-id="ec72b-146">String</span></span>|<span data-ttu-id="ec72b-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ec72b-147">The publisher of the app.</span></span> <span data-ttu-id="ec72b-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ec72b-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ec72b-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="ec72b-149">largeIcon</span></span>|[<span data-ttu-id="ec72b-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ec72b-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="ec72b-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="ec72b-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="ec72b-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ec72b-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ec72b-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ec72b-153">createdDateTime</span></span>|<span data-ttu-id="ec72b-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec72b-154">DateTimeOffset</span></span>|<span data-ttu-id="ec72b-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ec72b-155">The date and time the app was created.</span></span> <span data-ttu-id="ec72b-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ec72b-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ec72b-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ec72b-157">lastModifiedDateTime</span></span>|<span data-ttu-id="ec72b-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec72b-158">DateTimeOffset</span></span>|<span data-ttu-id="ec72b-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="ec72b-159">The date and time the app was last modified.</span></span> <span data-ttu-id="ec72b-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ec72b-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ec72b-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="ec72b-161">isFeatured</span></span>|<span data-ttu-id="ec72b-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec72b-162">Boolean</span></span>|<span data-ttu-id="ec72b-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ec72b-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ec72b-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="ec72b-164">privacyInformationUrl</span></span>|<span data-ttu-id="ec72b-165">String</span><span class="sxs-lookup"><span data-stu-id="ec72b-165">String</span></span>|<span data-ttu-id="ec72b-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="ec72b-166">The privacy statement Url.</span></span> <span data-ttu-id="ec72b-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ec72b-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ec72b-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="ec72b-168">informationUrl</span></span>|<span data-ttu-id="ec72b-169">String</span><span class="sxs-lookup"><span data-stu-id="ec72b-169">String</span></span>|<span data-ttu-id="ec72b-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="ec72b-170">The more information Url.</span></span> <span data-ttu-id="ec72b-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ec72b-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ec72b-172">owner</span><span class="sxs-lookup"><span data-stu-id="ec72b-172">owner</span></span>|<span data-ttu-id="ec72b-173">String</span><span class="sxs-lookup"><span data-stu-id="ec72b-173">String</span></span>|<span data-ttu-id="ec72b-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="ec72b-174">The owner of the app.</span></span> <span data-ttu-id="ec72b-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ec72b-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ec72b-176">developer</span><span class="sxs-lookup"><span data-stu-id="ec72b-176">developer</span></span>|<span data-ttu-id="ec72b-177">String</span><span class="sxs-lookup"><span data-stu-id="ec72b-177">String</span></span>|<span data-ttu-id="ec72b-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ec72b-178">The developer of the app.</span></span> <span data-ttu-id="ec72b-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ec72b-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ec72b-180">notes</span><span class="sxs-lookup"><span data-stu-id="ec72b-180">notes</span></span>|<span data-ttu-id="ec72b-181">String</span><span class="sxs-lookup"><span data-stu-id="ec72b-181">String</span></span>|<span data-ttu-id="ec72b-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ec72b-182">Notes for the app.</span></span> <span data-ttu-id="ec72b-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ec72b-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ec72b-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="ec72b-184">uploadState</span></span>|<span data-ttu-id="ec72b-185">Int32</span><span class="sxs-lookup"><span data-stu-id="ec72b-185">Int32</span></span>|<span data-ttu-id="ec72b-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="ec72b-186">The upload state.</span></span> <span data-ttu-id="ec72b-187">Os valores possíveis são: 0- `Not Ready` , 1- `Ready` , 2- `Processing` .</span><span class="sxs-lookup"><span data-stu-id="ec72b-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="ec72b-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ec72b-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ec72b-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="ec72b-189">publishingState</span></span>|[<span data-ttu-id="ec72b-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="ec72b-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="ec72b-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ec72b-191">The publishing state for the app.</span></span> <span data-ttu-id="ec72b-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="ec72b-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="ec72b-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ec72b-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="ec72b-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="ec72b-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="ec72b-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="ec72b-195">isAssigned</span></span>|<span data-ttu-id="ec72b-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec72b-196">Boolean</span></span>|<span data-ttu-id="ec72b-197">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="ec72b-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="ec72b-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ec72b-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ec72b-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ec72b-199">roleScopeTagIds</span></span>|<span data-ttu-id="ec72b-200">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ec72b-200">String collection</span></span>|<span data-ttu-id="ec72b-201">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="ec72b-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="ec72b-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ec72b-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ec72b-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="ec72b-203">dependentAppCount</span></span>|<span data-ttu-id="ec72b-204">Int32</span><span class="sxs-lookup"><span data-stu-id="ec72b-204">Int32</span></span>|<span data-ttu-id="ec72b-205">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="ec72b-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="ec72b-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ec72b-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ec72b-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="ec72b-207">supersedingAppCount</span></span>|<span data-ttu-id="ec72b-208">Int32</span><span class="sxs-lookup"><span data-stu-id="ec72b-208">Int32</span></span>|<span data-ttu-id="ec72b-209">O número total de aplicativos que este aplicativo substitui direta ou indiretamente.</span><span class="sxs-lookup"><span data-stu-id="ec72b-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="ec72b-210">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ec72b-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ec72b-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="ec72b-211">supersededAppCount</span></span>|<span data-ttu-id="ec72b-212">Int32</span><span class="sxs-lookup"><span data-stu-id="ec72b-212">Int32</span></span>|<span data-ttu-id="ec72b-213">O número total de aplicativos que este aplicativo está substituindo direta ou indiretamente por.</span><span class="sxs-lookup"><span data-stu-id="ec72b-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="ec72b-214">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ec72b-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ec72b-215">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="ec72b-215">committedContentVersion</span></span>|<span data-ttu-id="ec72b-216">String</span><span class="sxs-lookup"><span data-stu-id="ec72b-216">String</span></span>|<span data-ttu-id="ec72b-217">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="ec72b-217">The internal committed content version.</span></span> <span data-ttu-id="ec72b-218">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="ec72b-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="ec72b-219">fileName</span><span class="sxs-lookup"><span data-stu-id="ec72b-219">fileName</span></span>|<span data-ttu-id="ec72b-220">String</span><span class="sxs-lookup"><span data-stu-id="ec72b-220">String</span></span>|<span data-ttu-id="ec72b-221">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="ec72b-221">The name of the main Lob application file.</span></span> <span data-ttu-id="ec72b-222">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="ec72b-222">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="ec72b-223">size</span><span class="sxs-lookup"><span data-stu-id="ec72b-223">size</span></span>|<span data-ttu-id="ec72b-224">Int64</span><span class="sxs-lookup"><span data-stu-id="ec72b-224">Int64</span></span>|<span data-ttu-id="ec72b-225">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="ec72b-225">The total size, including all uploaded files.</span></span> <span data-ttu-id="ec72b-226">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="ec72b-226">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="ec72b-227">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="ec72b-227">applicableArchitectures</span></span>|[<span data-ttu-id="ec72b-228">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="ec72b-228">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="ec72b-229">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="ec72b-229">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="ec72b-230">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span><span class="sxs-lookup"><span data-stu-id="ec72b-230">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span></span> <span data-ttu-id="ec72b-231">Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="ec72b-231">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="ec72b-232">identityName</span><span class="sxs-lookup"><span data-stu-id="ec72b-232">identityName</span></span>|<span data-ttu-id="ec72b-233">String</span><span class="sxs-lookup"><span data-stu-id="ec72b-233">String</span></span>|<span data-ttu-id="ec72b-234">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="ec72b-234">The Identity Name.</span></span> <span data-ttu-id="ec72b-235">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="ec72b-235">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="ec72b-236">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="ec72b-236">identityPublisherHash</span></span>|<span data-ttu-id="ec72b-237">String</span><span class="sxs-lookup"><span data-stu-id="ec72b-237">String</span></span>|<span data-ttu-id="ec72b-238">O Hash do Publicador de Identidade.</span><span class="sxs-lookup"><span data-stu-id="ec72b-238">The Identity Publisher Hash.</span></span> <span data-ttu-id="ec72b-239">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="ec72b-239">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="ec72b-240">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="ec72b-240">identityResourceIdentifier</span></span>|<span data-ttu-id="ec72b-241">String</span><span class="sxs-lookup"><span data-stu-id="ec72b-241">String</span></span>|<span data-ttu-id="ec72b-242">O Identificador de Recurso da Identidade.</span><span class="sxs-lookup"><span data-stu-id="ec72b-242">The Identity Resource Identifier.</span></span> <span data-ttu-id="ec72b-243">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="ec72b-243">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="ec72b-244">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ec72b-244">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="ec72b-245">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ec72b-245">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="ec72b-246">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="ec72b-246">The value for the minimum applicable operating system.</span></span> <span data-ttu-id="ec72b-247">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="ec72b-247">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="ec72b-248">phoneProductIdentifier</span><span class="sxs-lookup"><span data-stu-id="ec72b-248">phoneProductIdentifier</span></span>|<span data-ttu-id="ec72b-249">String</span><span class="sxs-lookup"><span data-stu-id="ec72b-249">String</span></span>|<span data-ttu-id="ec72b-250">O identificador do produto de telefone.</span><span class="sxs-lookup"><span data-stu-id="ec72b-250">The Phone Product Identifier.</span></span> <span data-ttu-id="ec72b-251">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="ec72b-251">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="ec72b-252">phonePublisherId</span><span class="sxs-lookup"><span data-stu-id="ec72b-252">phonePublisherId</span></span>|<span data-ttu-id="ec72b-253">String</span><span class="sxs-lookup"><span data-stu-id="ec72b-253">String</span></span>|<span data-ttu-id="ec72b-254">A ID do editor do telefone. herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="ec72b-254">The Phone Publisher Id. Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="ec72b-255">identityVersion</span><span class="sxs-lookup"><span data-stu-id="ec72b-255">identityVersion</span></span>|<span data-ttu-id="ec72b-256">String</span><span class="sxs-lookup"><span data-stu-id="ec72b-256">String</span></span>|<span data-ttu-id="ec72b-257">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="ec72b-257">The identity version.</span></span> <span data-ttu-id="ec72b-258">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="ec72b-258">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="ec72b-259">appXPackageInformationList</span><span class="sxs-lookup"><span data-stu-id="ec72b-259">appXPackageInformationList</span></span>|<span data-ttu-id="ec72b-260">coleção [windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md)</span><span class="sxs-lookup"><span data-stu-id="ec72b-260">[windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md) collection</span></span>|<span data-ttu-id="ec72b-261">A lista de informações do pacote AppX.</span><span class="sxs-lookup"><span data-stu-id="ec72b-261">The list of AppX Package Information.</span></span>|



## <a name="response"></a><span data-ttu-id="ec72b-262">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec72b-262">Response</span></span>
<span data-ttu-id="ec72b-263">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ec72b-263">If successful, this method returns a `201 Created` response code and a [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec72b-264">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ec72b-264">Example</span></span>

### <a name="request"></a><span data-ttu-id="ec72b-265">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ec72b-265">Request</span></span>
<span data-ttu-id="ec72b-266">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ec72b-266">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="ec72b-267">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec72b-267">Response</span></span>
<span data-ttu-id="ec72b-p131">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ec72b-p131">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





