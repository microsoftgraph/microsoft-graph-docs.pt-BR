---
title: Criar windowsPhone81AppXBundle
description: Crie um novo objeto windowsPhone81AppXBundle.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 78743a394d6530d45637ef23028b8eb0a44afb87
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51862943"
---
# <a name="create-windowsphone81appxbundle"></a><span data-ttu-id="45494-103">Criar windowsPhone81AppXBundle</span><span class="sxs-lookup"><span data-stu-id="45494-103">Create windowsPhone81AppXBundle</span></span>

<span data-ttu-id="45494-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45494-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="45494-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="45494-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="45494-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="45494-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45494-107">Crie um novo [objeto windowsPhone81AppXBundle.](../resources/intune-apps-windowsphone81appxbundle.md)</span><span class="sxs-lookup"><span data-stu-id="45494-107">Create a new [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="45494-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="45494-108">Prerequisites</span></span>
<span data-ttu-id="45494-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45494-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45494-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="45494-111">Permission type</span></span>|<span data-ttu-id="45494-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="45494-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45494-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="45494-113">Delegated (work or school account)</span></span>|<span data-ttu-id="45494-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45494-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="45494-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="45494-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45494-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="45494-116">Not supported.</span></span>|
|<span data-ttu-id="45494-117">Application</span><span class="sxs-lookup"><span data-stu-id="45494-117">Application</span></span>|<span data-ttu-id="45494-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45494-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="45494-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="45494-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="45494-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="45494-120">Request headers</span></span>
|<span data-ttu-id="45494-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="45494-121">Header</span></span>|<span data-ttu-id="45494-122">Valor</span><span class="sxs-lookup"><span data-stu-id="45494-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45494-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="45494-123">Authorization</span></span>|<span data-ttu-id="45494-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="45494-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45494-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="45494-125">Accept</span></span>|<span data-ttu-id="45494-126">application/json</span><span class="sxs-lookup"><span data-stu-id="45494-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45494-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="45494-127">Request body</span></span>
<span data-ttu-id="45494-128">No corpo da solicitação, fornece uma representação JSON para o objeto windowsPhone81AppXBundle.</span><span class="sxs-lookup"><span data-stu-id="45494-128">In the request body, supply a JSON representation for the windowsPhone81AppXBundle object.</span></span>

<span data-ttu-id="45494-129">A tabela a seguir mostra as propriedades necessárias ao criar o windowsPhone81AppXBundle.</span><span class="sxs-lookup"><span data-stu-id="45494-129">The following table shows the properties that are required when you create the windowsPhone81AppXBundle.</span></span>

|<span data-ttu-id="45494-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="45494-130">Property</span></span>|<span data-ttu-id="45494-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="45494-131">Type</span></span>|<span data-ttu-id="45494-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="45494-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45494-133">id</span><span class="sxs-lookup"><span data-stu-id="45494-133">id</span></span>|<span data-ttu-id="45494-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="45494-134">String</span></span>|<span data-ttu-id="45494-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="45494-135">Key of the entity.</span></span> <span data-ttu-id="45494-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="45494-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="45494-137">displayName</span><span class="sxs-lookup"><span data-stu-id="45494-137">displayName</span></span>|<span data-ttu-id="45494-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="45494-138">String</span></span>|<span data-ttu-id="45494-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="45494-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="45494-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="45494-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="45494-141">description</span><span class="sxs-lookup"><span data-stu-id="45494-141">description</span></span>|<span data-ttu-id="45494-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="45494-142">String</span></span>|<span data-ttu-id="45494-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="45494-143">The description of the app.</span></span> <span data-ttu-id="45494-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="45494-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="45494-145">publicador</span><span class="sxs-lookup"><span data-stu-id="45494-145">publisher</span></span>|<span data-ttu-id="45494-146">String</span><span class="sxs-lookup"><span data-stu-id="45494-146">String</span></span>|<span data-ttu-id="45494-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="45494-147">The publisher of the app.</span></span> <span data-ttu-id="45494-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="45494-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="45494-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="45494-149">largeIcon</span></span>|[<span data-ttu-id="45494-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="45494-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="45494-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="45494-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="45494-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="45494-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="45494-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="45494-153">createdDateTime</span></span>|<span data-ttu-id="45494-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45494-154">DateTimeOffset</span></span>|<span data-ttu-id="45494-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="45494-155">The date and time the app was created.</span></span> <span data-ttu-id="45494-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="45494-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="45494-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="45494-157">lastModifiedDateTime</span></span>|<span data-ttu-id="45494-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45494-158">DateTimeOffset</span></span>|<span data-ttu-id="45494-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="45494-159">The date and time the app was last modified.</span></span> <span data-ttu-id="45494-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="45494-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="45494-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="45494-161">isFeatured</span></span>|<span data-ttu-id="45494-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="45494-162">Boolean</span></span>|<span data-ttu-id="45494-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="45494-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="45494-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="45494-164">privacyInformationUrl</span></span>|<span data-ttu-id="45494-165">String</span><span class="sxs-lookup"><span data-stu-id="45494-165">String</span></span>|<span data-ttu-id="45494-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="45494-166">The privacy statement Url.</span></span> <span data-ttu-id="45494-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="45494-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="45494-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="45494-168">informationUrl</span></span>|<span data-ttu-id="45494-169">String</span><span class="sxs-lookup"><span data-stu-id="45494-169">String</span></span>|<span data-ttu-id="45494-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="45494-170">The more information Url.</span></span> <span data-ttu-id="45494-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="45494-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="45494-172">owner</span><span class="sxs-lookup"><span data-stu-id="45494-172">owner</span></span>|<span data-ttu-id="45494-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="45494-173">String</span></span>|<span data-ttu-id="45494-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="45494-174">The owner of the app.</span></span> <span data-ttu-id="45494-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="45494-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="45494-176">developer</span><span class="sxs-lookup"><span data-stu-id="45494-176">developer</span></span>|<span data-ttu-id="45494-177">String</span><span class="sxs-lookup"><span data-stu-id="45494-177">String</span></span>|<span data-ttu-id="45494-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="45494-178">The developer of the app.</span></span> <span data-ttu-id="45494-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="45494-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="45494-180">notes</span><span class="sxs-lookup"><span data-stu-id="45494-180">notes</span></span>|<span data-ttu-id="45494-181">String</span><span class="sxs-lookup"><span data-stu-id="45494-181">String</span></span>|<span data-ttu-id="45494-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="45494-182">Notes for the app.</span></span> <span data-ttu-id="45494-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="45494-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="45494-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="45494-184">uploadState</span></span>|<span data-ttu-id="45494-185">Int32</span><span class="sxs-lookup"><span data-stu-id="45494-185">Int32</span></span>|<span data-ttu-id="45494-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="45494-186">The upload state.</span></span> <span data-ttu-id="45494-187">Os valores possíveis são: 0 - `Not Ready` , 1 - `Ready` , 2 - `Processing` .</span><span class="sxs-lookup"><span data-stu-id="45494-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="45494-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="45494-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="45494-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="45494-189">publishingState</span></span>|[<span data-ttu-id="45494-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="45494-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="45494-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="45494-191">The publishing state for the app.</span></span> <span data-ttu-id="45494-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="45494-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="45494-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="45494-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="45494-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="45494-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="45494-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="45494-195">isAssigned</span></span>|<span data-ttu-id="45494-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="45494-196">Boolean</span></span>|<span data-ttu-id="45494-197">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="45494-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="45494-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="45494-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="45494-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="45494-199">roleScopeTagIds</span></span>|<span data-ttu-id="45494-200">Coleção String</span><span class="sxs-lookup"><span data-stu-id="45494-200">String collection</span></span>|<span data-ttu-id="45494-201">Lista de ids de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="45494-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="45494-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="45494-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="45494-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="45494-203">dependentAppCount</span></span>|<span data-ttu-id="45494-204">Int32</span><span class="sxs-lookup"><span data-stu-id="45494-204">Int32</span></span>|<span data-ttu-id="45494-205">O número total de dependências que o aplicativo filho tem.</span><span class="sxs-lookup"><span data-stu-id="45494-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="45494-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="45494-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="45494-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="45494-207">supersedingAppCount</span></span>|<span data-ttu-id="45494-208">Int32</span><span class="sxs-lookup"><span data-stu-id="45494-208">Int32</span></span>|<span data-ttu-id="45494-209">O número total de aplicativos que esse aplicativo sobressede direta ou indiretamente.</span><span class="sxs-lookup"><span data-stu-id="45494-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="45494-210">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="45494-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="45494-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="45494-211">supersededAppCount</span></span>|<span data-ttu-id="45494-212">Int32</span><span class="sxs-lookup"><span data-stu-id="45494-212">Int32</span></span>|<span data-ttu-id="45494-213">O número total de aplicativos pelos quais esse aplicativo é, direta ou indiretamente, é suplido.</span><span class="sxs-lookup"><span data-stu-id="45494-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="45494-214">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="45494-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="45494-215">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="45494-215">committedContentVersion</span></span>|<span data-ttu-id="45494-216">String</span><span class="sxs-lookup"><span data-stu-id="45494-216">String</span></span>|<span data-ttu-id="45494-217">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="45494-217">The internal committed content version.</span></span> <span data-ttu-id="45494-218">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="45494-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="45494-219">fileName</span><span class="sxs-lookup"><span data-stu-id="45494-219">fileName</span></span>|<span data-ttu-id="45494-220">String</span><span class="sxs-lookup"><span data-stu-id="45494-220">String</span></span>|<span data-ttu-id="45494-221">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="45494-221">The name of the main Lob application file.</span></span> <span data-ttu-id="45494-222">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="45494-222">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="45494-223">size</span><span class="sxs-lookup"><span data-stu-id="45494-223">size</span></span>|<span data-ttu-id="45494-224">Int64</span><span class="sxs-lookup"><span data-stu-id="45494-224">Int64</span></span>|<span data-ttu-id="45494-225">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="45494-225">The total size, including all uploaded files.</span></span> <span data-ttu-id="45494-226">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="45494-226">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="45494-227">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="45494-227">applicableArchitectures</span></span>|[<span data-ttu-id="45494-228">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="45494-228">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="45494-229">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="45494-229">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="45494-230">Herdado do [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span><span class="sxs-lookup"><span data-stu-id="45494-230">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span></span> <span data-ttu-id="45494-231">Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="45494-231">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="45494-232">identityName</span><span class="sxs-lookup"><span data-stu-id="45494-232">identityName</span></span>|<span data-ttu-id="45494-233">String</span><span class="sxs-lookup"><span data-stu-id="45494-233">String</span></span>|<span data-ttu-id="45494-234">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="45494-234">The Identity Name.</span></span> <span data-ttu-id="45494-235">Herdado do [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="45494-235">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="45494-236">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="45494-236">identityPublisherHash</span></span>|<span data-ttu-id="45494-237">String</span><span class="sxs-lookup"><span data-stu-id="45494-237">String</span></span>|<span data-ttu-id="45494-238">O Hash do Publicador de Identidade.</span><span class="sxs-lookup"><span data-stu-id="45494-238">The Identity Publisher Hash.</span></span> <span data-ttu-id="45494-239">Herdado do [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="45494-239">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="45494-240">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="45494-240">identityResourceIdentifier</span></span>|<span data-ttu-id="45494-241">String</span><span class="sxs-lookup"><span data-stu-id="45494-241">String</span></span>|<span data-ttu-id="45494-242">O Identificador de Recurso da Identidade.</span><span class="sxs-lookup"><span data-stu-id="45494-242">The Identity Resource Identifier.</span></span> <span data-ttu-id="45494-243">Herdado do [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="45494-243">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="45494-244">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="45494-244">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="45494-245">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="45494-245">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="45494-246">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="45494-246">The value for the minimum applicable operating system.</span></span> <span data-ttu-id="45494-247">Herdado do [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="45494-247">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="45494-248">phoneProductIdentifier</span><span class="sxs-lookup"><span data-stu-id="45494-248">phoneProductIdentifier</span></span>|<span data-ttu-id="45494-249">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="45494-249">String</span></span>|<span data-ttu-id="45494-250">O Identificador de Produto de Telefone.</span><span class="sxs-lookup"><span data-stu-id="45494-250">The Phone Product Identifier.</span></span> <span data-ttu-id="45494-251">Herdado do [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="45494-251">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="45494-252">phonePublisherId</span><span class="sxs-lookup"><span data-stu-id="45494-252">phonePublisherId</span></span>|<span data-ttu-id="45494-253">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="45494-253">String</span></span>|<span data-ttu-id="45494-254">A ID do Editor de Telefones. Herdada do [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="45494-254">The Phone Publisher Id. Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="45494-255">identityVersion</span><span class="sxs-lookup"><span data-stu-id="45494-255">identityVersion</span></span>|<span data-ttu-id="45494-256">String</span><span class="sxs-lookup"><span data-stu-id="45494-256">String</span></span>|<span data-ttu-id="45494-257">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="45494-257">The identity version.</span></span> <span data-ttu-id="45494-258">Herdado do [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="45494-258">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="45494-259">appXPackageInformationList</span><span class="sxs-lookup"><span data-stu-id="45494-259">appXPackageInformationList</span></span>|<span data-ttu-id="45494-260">[Coleção windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md)</span><span class="sxs-lookup"><span data-stu-id="45494-260">[windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md) collection</span></span>|<span data-ttu-id="45494-261">A lista de Informações do Pacote AppX.</span><span class="sxs-lookup"><span data-stu-id="45494-261">The list of AppX Package Information.</span></span>|



## <a name="response"></a><span data-ttu-id="45494-262">Resposta</span><span class="sxs-lookup"><span data-stu-id="45494-262">Response</span></span>
<span data-ttu-id="45494-263">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="45494-263">If successful, this method returns a `201 Created` response code and a [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45494-264">Exemplo</span><span class="sxs-lookup"><span data-stu-id="45494-264">Example</span></span>

### <a name="request"></a><span data-ttu-id="45494-265">Solicitação</span><span class="sxs-lookup"><span data-stu-id="45494-265">Request</span></span>
<span data-ttu-id="45494-266">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="45494-266">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 2518

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
    "v10_2004": true,
    "v10_2H20": true
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
        "v10_2004": true,
        "v10_2H20": true
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="45494-267">Resposta</span><span class="sxs-lookup"><span data-stu-id="45494-267">Response</span></span>
<span data-ttu-id="45494-p131">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="45494-p131">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2690

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
    "v10_2004": true,
    "v10_2H20": true
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
        "v10_2004": true,
        "v10_2H20": true
      }
    }
  ]
}
```




