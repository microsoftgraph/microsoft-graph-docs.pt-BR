---
title: Criar windowsPhone81AppX
description: Crie um novo objeto windowsPhone81AppX.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6b906999bdbbe6c3fe87035ec0cc1881a411e24f
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156193"
---
# <a name="create-windowsphone81appx"></a><span data-ttu-id="6a98a-103">Criar windowsPhone81AppX</span><span class="sxs-lookup"><span data-stu-id="6a98a-103">Create windowsPhone81AppX</span></span>

<span data-ttu-id="6a98a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a98a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6a98a-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6a98a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a98a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6a98a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a98a-107">Crie um novo [objeto windowsPhone81AppX.](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="6a98a-107">Create a new [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6a98a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6a98a-108">Prerequisites</span></span>
<span data-ttu-id="6a98a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a98a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a98a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6a98a-111">Permission type</span></span>|<span data-ttu-id="6a98a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6a98a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a98a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6a98a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6a98a-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a98a-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6a98a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6a98a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a98a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6a98a-116">Not supported.</span></span>|
|<span data-ttu-id="6a98a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6a98a-117">Application</span></span>|<span data-ttu-id="6a98a-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a98a-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a98a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6a98a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="6a98a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6a98a-120">Request headers</span></span>
|<span data-ttu-id="6a98a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6a98a-121">Header</span></span>|<span data-ttu-id="6a98a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6a98a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6a98a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6a98a-123">Authorization</span></span>|<span data-ttu-id="6a98a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6a98a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6a98a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6a98a-125">Accept</span></span>|<span data-ttu-id="6a98a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6a98a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a98a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6a98a-127">Request body</span></span>
<span data-ttu-id="6a98a-128">No corpo da solicitação, fornece uma representação JSON do objeto windowsPhone81AppX.</span><span class="sxs-lookup"><span data-stu-id="6a98a-128">In the request body, supply a JSON representation for the windowsPhone81AppX object.</span></span>

<span data-ttu-id="6a98a-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsPhone81AppX.</span><span class="sxs-lookup"><span data-stu-id="6a98a-129">The following table shows the properties that are required when you create the windowsPhone81AppX.</span></span>

|<span data-ttu-id="6a98a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6a98a-130">Property</span></span>|<span data-ttu-id="6a98a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6a98a-131">Type</span></span>|<span data-ttu-id="6a98a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a98a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a98a-133">id</span><span class="sxs-lookup"><span data-stu-id="6a98a-133">id</span></span>|<span data-ttu-id="6a98a-134">String</span><span class="sxs-lookup"><span data-stu-id="6a98a-134">String</span></span>|<span data-ttu-id="6a98a-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6a98a-135">Key of the entity.</span></span> <span data-ttu-id="6a98a-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6a98a-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6a98a-137">displayName</span><span class="sxs-lookup"><span data-stu-id="6a98a-137">displayName</span></span>|<span data-ttu-id="6a98a-138">String</span><span class="sxs-lookup"><span data-stu-id="6a98a-138">String</span></span>|<span data-ttu-id="6a98a-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="6a98a-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="6a98a-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6a98a-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6a98a-141">description</span><span class="sxs-lookup"><span data-stu-id="6a98a-141">description</span></span>|<span data-ttu-id="6a98a-142">String</span><span class="sxs-lookup"><span data-stu-id="6a98a-142">String</span></span>|<span data-ttu-id="6a98a-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6a98a-143">The description of the app.</span></span> <span data-ttu-id="6a98a-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6a98a-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6a98a-145">publicador</span><span class="sxs-lookup"><span data-stu-id="6a98a-145">publisher</span></span>|<span data-ttu-id="6a98a-146">String</span><span class="sxs-lookup"><span data-stu-id="6a98a-146">String</span></span>|<span data-ttu-id="6a98a-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6a98a-147">The publisher of the app.</span></span> <span data-ttu-id="6a98a-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6a98a-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6a98a-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="6a98a-149">largeIcon</span></span>|[<span data-ttu-id="6a98a-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="6a98a-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="6a98a-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="6a98a-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="6a98a-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6a98a-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6a98a-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6a98a-153">createdDateTime</span></span>|<span data-ttu-id="6a98a-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a98a-154">DateTimeOffset</span></span>|<span data-ttu-id="6a98a-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6a98a-155">The date and time the app was created.</span></span> <span data-ttu-id="6a98a-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6a98a-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6a98a-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6a98a-157">lastModifiedDateTime</span></span>|<span data-ttu-id="6a98a-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a98a-158">DateTimeOffset</span></span>|<span data-ttu-id="6a98a-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="6a98a-159">The date and time the app was last modified.</span></span> <span data-ttu-id="6a98a-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6a98a-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6a98a-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="6a98a-161">isFeatured</span></span>|<span data-ttu-id="6a98a-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="6a98a-162">Boolean</span></span>|<span data-ttu-id="6a98a-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6a98a-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6a98a-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="6a98a-164">privacyInformationUrl</span></span>|<span data-ttu-id="6a98a-165">String</span><span class="sxs-lookup"><span data-stu-id="6a98a-165">String</span></span>|<span data-ttu-id="6a98a-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="6a98a-166">The privacy statement Url.</span></span> <span data-ttu-id="6a98a-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6a98a-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6a98a-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="6a98a-168">informationUrl</span></span>|<span data-ttu-id="6a98a-169">String</span><span class="sxs-lookup"><span data-stu-id="6a98a-169">String</span></span>|<span data-ttu-id="6a98a-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="6a98a-170">The more information Url.</span></span> <span data-ttu-id="6a98a-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6a98a-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6a98a-172">owner</span><span class="sxs-lookup"><span data-stu-id="6a98a-172">owner</span></span>|<span data-ttu-id="6a98a-173">String</span><span class="sxs-lookup"><span data-stu-id="6a98a-173">String</span></span>|<span data-ttu-id="6a98a-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="6a98a-174">The owner of the app.</span></span> <span data-ttu-id="6a98a-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6a98a-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6a98a-176">developer</span><span class="sxs-lookup"><span data-stu-id="6a98a-176">developer</span></span>|<span data-ttu-id="6a98a-177">String</span><span class="sxs-lookup"><span data-stu-id="6a98a-177">String</span></span>|<span data-ttu-id="6a98a-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6a98a-178">The developer of the app.</span></span> <span data-ttu-id="6a98a-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6a98a-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6a98a-180">notes</span><span class="sxs-lookup"><span data-stu-id="6a98a-180">notes</span></span>|<span data-ttu-id="6a98a-181">String</span><span class="sxs-lookup"><span data-stu-id="6a98a-181">String</span></span>|<span data-ttu-id="6a98a-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6a98a-182">Notes for the app.</span></span> <span data-ttu-id="6a98a-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6a98a-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6a98a-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="6a98a-184">uploadState</span></span>|<span data-ttu-id="6a98a-185">Int32</span><span class="sxs-lookup"><span data-stu-id="6a98a-185">Int32</span></span>|<span data-ttu-id="6a98a-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="6a98a-186">The upload state.</span></span> <span data-ttu-id="6a98a-187">Os valores possíveis são: 0 - `Not Ready` , 1 - `Ready` , 2 - `Processing` .</span><span class="sxs-lookup"><span data-stu-id="6a98a-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="6a98a-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6a98a-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6a98a-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="6a98a-189">publishingState</span></span>|[<span data-ttu-id="6a98a-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="6a98a-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="6a98a-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6a98a-191">The publishing state for the app.</span></span> <span data-ttu-id="6a98a-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="6a98a-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="6a98a-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6a98a-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="6a98a-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="6a98a-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="6a98a-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="6a98a-195">isAssigned</span></span>|<span data-ttu-id="6a98a-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="6a98a-196">Boolean</span></span>|<span data-ttu-id="6a98a-197">O valor que indica se o aplicativo está atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="6a98a-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="6a98a-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6a98a-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6a98a-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6a98a-199">roleScopeTagIds</span></span>|<span data-ttu-id="6a98a-200">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6a98a-200">String collection</span></span>|<span data-ttu-id="6a98a-201">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="6a98a-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="6a98a-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6a98a-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6a98a-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="6a98a-203">dependentAppCount</span></span>|<span data-ttu-id="6a98a-204">Int32</span><span class="sxs-lookup"><span data-stu-id="6a98a-204">Int32</span></span>|<span data-ttu-id="6a98a-205">O número total de dependências que o aplicativo filho tem.</span><span class="sxs-lookup"><span data-stu-id="6a98a-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="6a98a-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6a98a-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6a98a-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="6a98a-207">supersedingAppCount</span></span>|<span data-ttu-id="6a98a-208">Int32</span><span class="sxs-lookup"><span data-stu-id="6a98a-208">Int32</span></span>|<span data-ttu-id="6a98a-209">O número total de aplicativos que este aplicativo é direta ou indiretamente é supersedido.</span><span class="sxs-lookup"><span data-stu-id="6a98a-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="6a98a-210">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6a98a-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6a98a-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="6a98a-211">supersededAppCount</span></span>|<span data-ttu-id="6a98a-212">Int32</span><span class="sxs-lookup"><span data-stu-id="6a98a-212">Int32</span></span>|<span data-ttu-id="6a98a-213">O número total de aplicativos pelos quais esse aplicativo é direta ou indiretamente sobressu valorado.</span><span class="sxs-lookup"><span data-stu-id="6a98a-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="6a98a-214">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6a98a-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6a98a-215">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="6a98a-215">committedContentVersion</span></span>|<span data-ttu-id="6a98a-216">String</span><span class="sxs-lookup"><span data-stu-id="6a98a-216">String</span></span>|<span data-ttu-id="6a98a-217">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="6a98a-217">The internal committed content version.</span></span> <span data-ttu-id="6a98a-218">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="6a98a-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="6a98a-219">fileName</span><span class="sxs-lookup"><span data-stu-id="6a98a-219">fileName</span></span>|<span data-ttu-id="6a98a-220">String</span><span class="sxs-lookup"><span data-stu-id="6a98a-220">String</span></span>|<span data-ttu-id="6a98a-221">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="6a98a-221">The name of the main Lob application file.</span></span> <span data-ttu-id="6a98a-222">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="6a98a-222">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="6a98a-223">size</span><span class="sxs-lookup"><span data-stu-id="6a98a-223">size</span></span>|<span data-ttu-id="6a98a-224">Int64</span><span class="sxs-lookup"><span data-stu-id="6a98a-224">Int64</span></span>|<span data-ttu-id="6a98a-225">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="6a98a-225">The total size, including all uploaded files.</span></span> <span data-ttu-id="6a98a-226">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="6a98a-226">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="6a98a-227">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="6a98a-227">applicableArchitectures</span></span>|[<span data-ttu-id="6a98a-228">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="6a98a-228">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="6a98a-229">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="6a98a-229">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="6a98a-230">Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="6a98a-230">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="6a98a-231">identityName</span><span class="sxs-lookup"><span data-stu-id="6a98a-231">identityName</span></span>|<span data-ttu-id="6a98a-232">String</span><span class="sxs-lookup"><span data-stu-id="6a98a-232">String</span></span>|<span data-ttu-id="6a98a-233">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="6a98a-233">The Identity Name.</span></span>|
|<span data-ttu-id="6a98a-234">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="6a98a-234">identityPublisherHash</span></span>|<span data-ttu-id="6a98a-235">String</span><span class="sxs-lookup"><span data-stu-id="6a98a-235">String</span></span>|<span data-ttu-id="6a98a-236">O Hash do Publicador de Identidade.</span><span class="sxs-lookup"><span data-stu-id="6a98a-236">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="6a98a-237">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="6a98a-237">identityResourceIdentifier</span></span>|<span data-ttu-id="6a98a-238">String</span><span class="sxs-lookup"><span data-stu-id="6a98a-238">String</span></span>|<span data-ttu-id="6a98a-239">O Identificador de Recurso da Identidade.</span><span class="sxs-lookup"><span data-stu-id="6a98a-239">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="6a98a-240">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="6a98a-240">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="6a98a-241">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="6a98a-241">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="6a98a-242">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="6a98a-242">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="6a98a-243">phoneProductIdentifier</span><span class="sxs-lookup"><span data-stu-id="6a98a-243">phoneProductIdentifier</span></span>|<span data-ttu-id="6a98a-244">String</span><span class="sxs-lookup"><span data-stu-id="6a98a-244">String</span></span>|<span data-ttu-id="6a98a-245">O Identificador de Produto de Telefone.</span><span class="sxs-lookup"><span data-stu-id="6a98a-245">The Phone Product Identifier.</span></span>|
|<span data-ttu-id="6a98a-246">phonePublisherId</span><span class="sxs-lookup"><span data-stu-id="6a98a-246">phonePublisherId</span></span>|<span data-ttu-id="6a98a-247">String</span><span class="sxs-lookup"><span data-stu-id="6a98a-247">String</span></span>|<span data-ttu-id="6a98a-248">A ID do Editor de Telefones.</span><span class="sxs-lookup"><span data-stu-id="6a98a-248">The Phone Publisher Id.</span></span>|
|<span data-ttu-id="6a98a-249">identityVersion</span><span class="sxs-lookup"><span data-stu-id="6a98a-249">identityVersion</span></span>|<span data-ttu-id="6a98a-250">String</span><span class="sxs-lookup"><span data-stu-id="6a98a-250">String</span></span>|<span data-ttu-id="6a98a-251">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="6a98a-251">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="6a98a-252">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a98a-252">Response</span></span>
<span data-ttu-id="6a98a-253">Se bem-sucedido, este método retorna um código de resposta e um objeto `201 Created` [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6a98a-253">If successful, this method returns a `201 Created` response code and a [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a98a-254">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6a98a-254">Example</span></span>

### <a name="request"></a><span data-ttu-id="6a98a-255">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6a98a-255">Request</span></span>
<span data-ttu-id="6a98a-256">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6a98a-256">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1616

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
    "v10_2004": true
  },
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="6a98a-257">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a98a-257">Response</span></span>
<span data-ttu-id="6a98a-p125">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6a98a-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1788

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
    "v10_2004": true
  },
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value"
}
```




