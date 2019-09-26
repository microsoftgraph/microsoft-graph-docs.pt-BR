---
title: Criar windowsPhone81AppXBundle
description: Criar um novo objeto windowsPhone81AppXBundle.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c0b72be1100b28dcb3ddbac10accc7a3782505f1
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37176937"
---
# <a name="create-windowsphone81appxbundle"></a><span data-ttu-id="cbba0-103">Criar windowsPhone81AppXBundle</span><span class="sxs-lookup"><span data-stu-id="cbba0-103">Create windowsPhone81AppXBundle</span></span>

> <span data-ttu-id="cbba0-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cbba0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cbba0-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cbba0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cbba0-106">Criar um novo objeto [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) .</span><span class="sxs-lookup"><span data-stu-id="cbba0-106">Create a new [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cbba0-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cbba0-107">Prerequisites</span></span>
<span data-ttu-id="cbba0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cbba0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cbba0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cbba0-110">Permission type</span></span>|<span data-ttu-id="cbba0-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cbba0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cbba0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cbba0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cbba0-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cbba0-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cbba0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cbba0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cbba0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cbba0-115">Not supported.</span></span>|
|<span data-ttu-id="cbba0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cbba0-116">Application</span></span>|<span data-ttu-id="cbba0-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cbba0-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cbba0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cbba0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="cbba0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cbba0-119">Request headers</span></span>
|<span data-ttu-id="cbba0-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cbba0-120">Header</span></span>|<span data-ttu-id="cbba0-121">Valor</span><span class="sxs-lookup"><span data-stu-id="cbba0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cbba0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="cbba0-122">Authorization</span></span>|<span data-ttu-id="cbba0-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cbba0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cbba0-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cbba0-124">Accept</span></span>|<span data-ttu-id="cbba0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cbba0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cbba0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cbba0-126">Request body</span></span>
<span data-ttu-id="cbba0-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsPhone81AppXBundle.</span><span class="sxs-lookup"><span data-stu-id="cbba0-127">In the request body, supply a JSON representation for the windowsPhone81AppXBundle object.</span></span>

<span data-ttu-id="cbba0-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsPhone81AppXBundle.</span><span class="sxs-lookup"><span data-stu-id="cbba0-128">The following table shows the properties that are required when you create the windowsPhone81AppXBundle.</span></span>

|<span data-ttu-id="cbba0-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cbba0-129">Property</span></span>|<span data-ttu-id="cbba0-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="cbba0-130">Type</span></span>|<span data-ttu-id="cbba0-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="cbba0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cbba0-132">id</span><span class="sxs-lookup"><span data-stu-id="cbba0-132">id</span></span>|<span data-ttu-id="cbba0-133">String</span><span class="sxs-lookup"><span data-stu-id="cbba0-133">String</span></span>|<span data-ttu-id="cbba0-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="cbba0-134">Key of the entity.</span></span> <span data-ttu-id="cbba0-135">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cbba0-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cbba0-136">displayName</span><span class="sxs-lookup"><span data-stu-id="cbba0-136">displayName</span></span>|<span data-ttu-id="cbba0-137">String</span><span class="sxs-lookup"><span data-stu-id="cbba0-137">String</span></span>|<span data-ttu-id="cbba0-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="cbba0-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="cbba0-139">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cbba0-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cbba0-140">descrição</span><span class="sxs-lookup"><span data-stu-id="cbba0-140">description</span></span>|<span data-ttu-id="cbba0-141">String</span><span class="sxs-lookup"><span data-stu-id="cbba0-141">String</span></span>|<span data-ttu-id="cbba0-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cbba0-142">The description of the app.</span></span> <span data-ttu-id="cbba0-143">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cbba0-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cbba0-144">publicador</span><span class="sxs-lookup"><span data-stu-id="cbba0-144">publisher</span></span>|<span data-ttu-id="cbba0-145">String</span><span class="sxs-lookup"><span data-stu-id="cbba0-145">String</span></span>|<span data-ttu-id="cbba0-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cbba0-146">The publisher of the app.</span></span> <span data-ttu-id="cbba0-147">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cbba0-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cbba0-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="cbba0-148">largeIcon</span></span>|[<span data-ttu-id="cbba0-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="cbba0-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="cbba0-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="cbba0-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="cbba0-151">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cbba0-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cbba0-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cbba0-152">createdDateTime</span></span>|<span data-ttu-id="cbba0-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cbba0-153">DateTimeOffset</span></span>|<span data-ttu-id="cbba0-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cbba0-154">The date and time the app was created.</span></span> <span data-ttu-id="cbba0-155">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cbba0-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cbba0-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cbba0-156">lastModifiedDateTime</span></span>|<span data-ttu-id="cbba0-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cbba0-157">DateTimeOffset</span></span>|<span data-ttu-id="cbba0-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="cbba0-158">The date and time the app was last modified.</span></span> <span data-ttu-id="cbba0-159">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cbba0-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cbba0-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="cbba0-160">isFeatured</span></span>|<span data-ttu-id="cbba0-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="cbba0-161">Boolean</span></span>|<span data-ttu-id="cbba0-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cbba0-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cbba0-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="cbba0-163">privacyInformationUrl</span></span>|<span data-ttu-id="cbba0-164">String</span><span class="sxs-lookup"><span data-stu-id="cbba0-164">String</span></span>|<span data-ttu-id="cbba0-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="cbba0-165">The privacy statement Url.</span></span> <span data-ttu-id="cbba0-166">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cbba0-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cbba0-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="cbba0-167">informationUrl</span></span>|<span data-ttu-id="cbba0-168">String</span><span class="sxs-lookup"><span data-stu-id="cbba0-168">String</span></span>|<span data-ttu-id="cbba0-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="cbba0-169">The more information Url.</span></span> <span data-ttu-id="cbba0-170">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cbba0-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cbba0-171">owner</span><span class="sxs-lookup"><span data-stu-id="cbba0-171">owner</span></span>|<span data-ttu-id="cbba0-172">String</span><span class="sxs-lookup"><span data-stu-id="cbba0-172">String</span></span>|<span data-ttu-id="cbba0-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="cbba0-173">The owner of the app.</span></span> <span data-ttu-id="cbba0-174">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cbba0-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cbba0-175">developer</span><span class="sxs-lookup"><span data-stu-id="cbba0-175">developer</span></span>|<span data-ttu-id="cbba0-176">String</span><span class="sxs-lookup"><span data-stu-id="cbba0-176">String</span></span>|<span data-ttu-id="cbba0-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cbba0-177">The developer of the app.</span></span> <span data-ttu-id="cbba0-178">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cbba0-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cbba0-179">notes</span><span class="sxs-lookup"><span data-stu-id="cbba0-179">notes</span></span>|<span data-ttu-id="cbba0-180">String</span><span class="sxs-lookup"><span data-stu-id="cbba0-180">String</span></span>|<span data-ttu-id="cbba0-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cbba0-181">Notes for the app.</span></span> <span data-ttu-id="cbba0-182">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cbba0-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cbba0-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="cbba0-183">uploadState</span></span>|<span data-ttu-id="cbba0-184">Int32</span><span class="sxs-lookup"><span data-stu-id="cbba0-184">Int32</span></span>|<span data-ttu-id="cbba0-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="cbba0-185">The upload state.</span></span> <span data-ttu-id="cbba0-186">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cbba0-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cbba0-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="cbba0-187">publishingState</span></span>|[<span data-ttu-id="cbba0-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="cbba0-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="cbba0-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cbba0-189">The publishing state for the app.</span></span> <span data-ttu-id="cbba0-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="cbba0-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="cbba0-191">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cbba0-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="cbba0-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="cbba0-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="cbba0-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="cbba0-193">isAssigned</span></span>|<span data-ttu-id="cbba0-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="cbba0-194">Boolean</span></span>|<span data-ttu-id="cbba0-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="cbba0-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="cbba0-196">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cbba0-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cbba0-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="cbba0-197">roleScopeTagIds</span></span>|<span data-ttu-id="cbba0-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="cbba0-198">String collection</span></span>|<span data-ttu-id="cbba0-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="cbba0-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="cbba0-200">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cbba0-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cbba0-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="cbba0-201">dependentAppCount</span></span>|<span data-ttu-id="cbba0-202">Int32</span><span class="sxs-lookup"><span data-stu-id="cbba0-202">Int32</span></span>|<span data-ttu-id="cbba0-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="cbba0-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="cbba0-204">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cbba0-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="cbba0-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="cbba0-205">committedContentVersion</span></span>|<span data-ttu-id="cbba0-206">String</span><span class="sxs-lookup"><span data-stu-id="cbba0-206">String</span></span>|<span data-ttu-id="cbba0-207">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="cbba0-207">The internal committed content version.</span></span> <span data-ttu-id="cbba0-208">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="cbba0-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="cbba0-209">fileName</span><span class="sxs-lookup"><span data-stu-id="cbba0-209">fileName</span></span>|<span data-ttu-id="cbba0-210">String</span><span class="sxs-lookup"><span data-stu-id="cbba0-210">String</span></span>|<span data-ttu-id="cbba0-211">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="cbba0-211">The name of the main Lob application file.</span></span> <span data-ttu-id="cbba0-212">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="cbba0-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="cbba0-213">size</span><span class="sxs-lookup"><span data-stu-id="cbba0-213">size</span></span>|<span data-ttu-id="cbba0-214">Int64</span><span class="sxs-lookup"><span data-stu-id="cbba0-214">Int64</span></span>|<span data-ttu-id="cbba0-215">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="cbba0-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="cbba0-216">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="cbba0-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="cbba0-217">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="cbba0-217">applicableArchitectures</span></span>|[<span data-ttu-id="cbba0-218">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="cbba0-218">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="cbba0-219">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="cbba0-219">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="cbba0-220">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span><span class="sxs-lookup"><span data-stu-id="cbba0-220">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span></span> <span data-ttu-id="cbba0-221">Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="cbba0-221">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="cbba0-222">identityName</span><span class="sxs-lookup"><span data-stu-id="cbba0-222">identityName</span></span>|<span data-ttu-id="cbba0-223">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cbba0-223">String</span></span>|<span data-ttu-id="cbba0-224">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="cbba0-224">The Identity Name.</span></span> <span data-ttu-id="cbba0-225">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="cbba0-225">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="cbba0-226">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="cbba0-226">identityPublisherHash</span></span>|<span data-ttu-id="cbba0-227">String</span><span class="sxs-lookup"><span data-stu-id="cbba0-227">String</span></span>|<span data-ttu-id="cbba0-228">O Hash do Publicador de Identidade.</span><span class="sxs-lookup"><span data-stu-id="cbba0-228">The Identity Publisher Hash.</span></span> <span data-ttu-id="cbba0-229">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="cbba0-229">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="cbba0-230">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="cbba0-230">identityResourceIdentifier</span></span>|<span data-ttu-id="cbba0-231">String</span><span class="sxs-lookup"><span data-stu-id="cbba0-231">String</span></span>|<span data-ttu-id="cbba0-232">O Identificador de Recurso da Identidade.</span><span class="sxs-lookup"><span data-stu-id="cbba0-232">The Identity Resource Identifier.</span></span> <span data-ttu-id="cbba0-233">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="cbba0-233">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="cbba0-234">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="cbba0-234">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="cbba0-235">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="cbba0-235">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="cbba0-236">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="cbba0-236">The value for the minimum applicable operating system.</span></span> <span data-ttu-id="cbba0-237">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="cbba0-237">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="cbba0-238">phoneProductIdentifier</span><span class="sxs-lookup"><span data-stu-id="cbba0-238">phoneProductIdentifier</span></span>|<span data-ttu-id="cbba0-239">String</span><span class="sxs-lookup"><span data-stu-id="cbba0-239">String</span></span>|<span data-ttu-id="cbba0-240">O identificador do produto de telefone.</span><span class="sxs-lookup"><span data-stu-id="cbba0-240">The Phone Product Identifier.</span></span> <span data-ttu-id="cbba0-241">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="cbba0-241">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="cbba0-242">phonePublisherId</span><span class="sxs-lookup"><span data-stu-id="cbba0-242">phonePublisherId</span></span>|<span data-ttu-id="cbba0-243">String</span><span class="sxs-lookup"><span data-stu-id="cbba0-243">String</span></span>|<span data-ttu-id="cbba0-244">A ID do editor do telefone. herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="cbba0-244">The Phone Publisher Id. Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="cbba0-245">identityVersion</span><span class="sxs-lookup"><span data-stu-id="cbba0-245">identityVersion</span></span>|<span data-ttu-id="cbba0-246">String</span><span class="sxs-lookup"><span data-stu-id="cbba0-246">String</span></span>|<span data-ttu-id="cbba0-247">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="cbba0-247">The identity version.</span></span> <span data-ttu-id="cbba0-248">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="cbba0-248">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="cbba0-249">appXPackageInformationList</span><span class="sxs-lookup"><span data-stu-id="cbba0-249">appXPackageInformationList</span></span>|<span data-ttu-id="cbba0-250">coleção [windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md)</span><span class="sxs-lookup"><span data-stu-id="cbba0-250">[windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md) collection</span></span>|<span data-ttu-id="cbba0-251">A lista de informações do pacote AppX.</span><span class="sxs-lookup"><span data-stu-id="cbba0-251">The list of AppX Package Information.</span></span>|



## <a name="response"></a><span data-ttu-id="cbba0-252">Resposta</span><span class="sxs-lookup"><span data-stu-id="cbba0-252">Response</span></span>
<span data-ttu-id="cbba0-253">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cbba0-253">If successful, this method returns a `201 Created` response code and a [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cbba0-254">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cbba0-254">Example</span></span>

### <a name="request"></a><span data-ttu-id="cbba0-255">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cbba0-255">Request</span></span>
<span data-ttu-id="cbba0-256">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cbba0-256">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 2311

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

### <a name="response"></a><span data-ttu-id="cbba0-257">Resposta</span><span class="sxs-lookup"><span data-stu-id="cbba0-257">Response</span></span>
<span data-ttu-id="cbba0-p129">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cbba0-p129">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2483

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




