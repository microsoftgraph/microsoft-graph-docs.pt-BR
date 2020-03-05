---
title: Criar windowsUniversalAppX
description: Cria um novo objeto windowsUniversalAppX.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ee60352d1167dbab17b82a50b672b0327e8b654e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42444676"
---
# <a name="create-windowsuniversalappx"></a><span data-ttu-id="8efd0-103">Criar windowsUniversalAppX</span><span class="sxs-lookup"><span data-stu-id="8efd0-103">Create windowsUniversalAppX</span></span>

<span data-ttu-id="8efd0-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="8efd0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8efd0-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8efd0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8efd0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8efd0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8efd0-107">Cria um novo objeto [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="8efd0-107">Create a new [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8efd0-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8efd0-108">Prerequisites</span></span>
<span data-ttu-id="8efd0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8efd0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8efd0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8efd0-111">Permission type</span></span>|<span data-ttu-id="8efd0-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8efd0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8efd0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8efd0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8efd0-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8efd0-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8efd0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8efd0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8efd0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8efd0-116">Not supported.</span></span>|
|<span data-ttu-id="8efd0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8efd0-117">Application</span></span>|<span data-ttu-id="8efd0-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8efd0-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8efd0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8efd0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="8efd0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8efd0-120">Request headers</span></span>
|<span data-ttu-id="8efd0-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8efd0-121">Header</span></span>|<span data-ttu-id="8efd0-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8efd0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8efd0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8efd0-123">Authorization</span></span>|<span data-ttu-id="8efd0-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8efd0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8efd0-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8efd0-125">Accept</span></span>|<span data-ttu-id="8efd0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8efd0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8efd0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8efd0-127">Request body</span></span>
<span data-ttu-id="8efd0-128">No corpo da solicitação, forneça uma representação JSON do objeto windowsUniversalAppX.</span><span class="sxs-lookup"><span data-stu-id="8efd0-128">In the request body, supply a JSON representation for the windowsUniversalAppX object.</span></span>

<span data-ttu-id="8efd0-129">A tabela a seguir mostra as propriedades obrigatórias ao criar windowsUniversalAppX.</span><span class="sxs-lookup"><span data-stu-id="8efd0-129">The following table shows the properties that are required when you create the windowsUniversalAppX.</span></span>

|<span data-ttu-id="8efd0-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8efd0-130">Property</span></span>|<span data-ttu-id="8efd0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8efd0-131">Type</span></span>|<span data-ttu-id="8efd0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8efd0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8efd0-133">id</span><span class="sxs-lookup"><span data-stu-id="8efd0-133">id</span></span>|<span data-ttu-id="8efd0-134">String</span><span class="sxs-lookup"><span data-stu-id="8efd0-134">String</span></span>|<span data-ttu-id="8efd0-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="8efd0-135">Key of the entity.</span></span> <span data-ttu-id="8efd0-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8efd0-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8efd0-137">displayName</span><span class="sxs-lookup"><span data-stu-id="8efd0-137">displayName</span></span>|<span data-ttu-id="8efd0-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8efd0-138">String</span></span>|<span data-ttu-id="8efd0-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="8efd0-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="8efd0-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8efd0-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8efd0-141">description</span><span class="sxs-lookup"><span data-stu-id="8efd0-141">description</span></span>|<span data-ttu-id="8efd0-142">String</span><span class="sxs-lookup"><span data-stu-id="8efd0-142">String</span></span>|<span data-ttu-id="8efd0-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8efd0-143">The description of the app.</span></span> <span data-ttu-id="8efd0-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8efd0-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8efd0-145">publicador</span><span class="sxs-lookup"><span data-stu-id="8efd0-145">publisher</span></span>|<span data-ttu-id="8efd0-146">String</span><span class="sxs-lookup"><span data-stu-id="8efd0-146">String</span></span>|<span data-ttu-id="8efd0-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8efd0-147">The publisher of the app.</span></span> <span data-ttu-id="8efd0-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8efd0-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8efd0-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="8efd0-149">largeIcon</span></span>|[<span data-ttu-id="8efd0-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="8efd0-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="8efd0-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="8efd0-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="8efd0-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8efd0-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8efd0-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8efd0-153">createdDateTime</span></span>|<span data-ttu-id="8efd0-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8efd0-154">DateTimeOffset</span></span>|<span data-ttu-id="8efd0-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8efd0-155">The date and time the app was created.</span></span> <span data-ttu-id="8efd0-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8efd0-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8efd0-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8efd0-157">lastModifiedDateTime</span></span>|<span data-ttu-id="8efd0-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8efd0-158">DateTimeOffset</span></span>|<span data-ttu-id="8efd0-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="8efd0-159">The date and time the app was last modified.</span></span> <span data-ttu-id="8efd0-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8efd0-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8efd0-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="8efd0-161">isFeatured</span></span>|<span data-ttu-id="8efd0-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="8efd0-162">Boolean</span></span>|<span data-ttu-id="8efd0-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8efd0-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8efd0-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="8efd0-164">privacyInformationUrl</span></span>|<span data-ttu-id="8efd0-165">String</span><span class="sxs-lookup"><span data-stu-id="8efd0-165">String</span></span>|<span data-ttu-id="8efd0-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="8efd0-166">The privacy statement Url.</span></span> <span data-ttu-id="8efd0-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8efd0-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8efd0-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="8efd0-168">informationUrl</span></span>|<span data-ttu-id="8efd0-169">String</span><span class="sxs-lookup"><span data-stu-id="8efd0-169">String</span></span>|<span data-ttu-id="8efd0-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="8efd0-170">The more information Url.</span></span> <span data-ttu-id="8efd0-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8efd0-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8efd0-172">owner</span><span class="sxs-lookup"><span data-stu-id="8efd0-172">owner</span></span>|<span data-ttu-id="8efd0-173">String</span><span class="sxs-lookup"><span data-stu-id="8efd0-173">String</span></span>|<span data-ttu-id="8efd0-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="8efd0-174">The owner of the app.</span></span> <span data-ttu-id="8efd0-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8efd0-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8efd0-176">developer</span><span class="sxs-lookup"><span data-stu-id="8efd0-176">developer</span></span>|<span data-ttu-id="8efd0-177">String</span><span class="sxs-lookup"><span data-stu-id="8efd0-177">String</span></span>|<span data-ttu-id="8efd0-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8efd0-178">The developer of the app.</span></span> <span data-ttu-id="8efd0-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8efd0-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8efd0-180">notes</span><span class="sxs-lookup"><span data-stu-id="8efd0-180">notes</span></span>|<span data-ttu-id="8efd0-181">String</span><span class="sxs-lookup"><span data-stu-id="8efd0-181">String</span></span>|<span data-ttu-id="8efd0-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8efd0-182">Notes for the app.</span></span> <span data-ttu-id="8efd0-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8efd0-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8efd0-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="8efd0-184">uploadState</span></span>|<span data-ttu-id="8efd0-185">Int32</span><span class="sxs-lookup"><span data-stu-id="8efd0-185">Int32</span></span>|<span data-ttu-id="8efd0-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="8efd0-186">The upload state.</span></span> <span data-ttu-id="8efd0-187">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8efd0-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8efd0-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="8efd0-188">publishingState</span></span>|[<span data-ttu-id="8efd0-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="8efd0-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="8efd0-190">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8efd0-190">The publishing state for the app.</span></span> <span data-ttu-id="8efd0-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="8efd0-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="8efd0-192">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8efd0-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="8efd0-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="8efd0-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="8efd0-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="8efd0-194">isAssigned</span></span>|<span data-ttu-id="8efd0-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="8efd0-195">Boolean</span></span>|<span data-ttu-id="8efd0-196">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="8efd0-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="8efd0-197">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8efd0-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8efd0-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8efd0-198">roleScopeTagIds</span></span>|<span data-ttu-id="8efd0-199">String collection</span><span class="sxs-lookup"><span data-stu-id="8efd0-199">String collection</span></span>|<span data-ttu-id="8efd0-200">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="8efd0-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="8efd0-201">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8efd0-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8efd0-202">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="8efd0-202">dependentAppCount</span></span>|<span data-ttu-id="8efd0-203">Int32</span><span class="sxs-lookup"><span data-stu-id="8efd0-203">Int32</span></span>|<span data-ttu-id="8efd0-204">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="8efd0-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="8efd0-205">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8efd0-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8efd0-206">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="8efd0-206">committedContentVersion</span></span>|<span data-ttu-id="8efd0-207">String</span><span class="sxs-lookup"><span data-stu-id="8efd0-207">String</span></span>|<span data-ttu-id="8efd0-208">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="8efd0-208">The internal committed content version.</span></span> <span data-ttu-id="8efd0-209">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="8efd0-209">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="8efd0-210">fileName</span><span class="sxs-lookup"><span data-stu-id="8efd0-210">fileName</span></span>|<span data-ttu-id="8efd0-211">String</span><span class="sxs-lookup"><span data-stu-id="8efd0-211">String</span></span>|<span data-ttu-id="8efd0-212">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="8efd0-212">The name of the main Lob application file.</span></span> <span data-ttu-id="8efd0-213">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="8efd0-213">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="8efd0-214">size</span><span class="sxs-lookup"><span data-stu-id="8efd0-214">size</span></span>|<span data-ttu-id="8efd0-215">Int64</span><span class="sxs-lookup"><span data-stu-id="8efd0-215">Int64</span></span>|<span data-ttu-id="8efd0-216">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="8efd0-216">The total size, including all uploaded files.</span></span> <span data-ttu-id="8efd0-217">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="8efd0-217">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="8efd0-218">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="8efd0-218">applicableArchitectures</span></span>|[<span data-ttu-id="8efd0-219">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="8efd0-219">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="8efd0-220">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="8efd0-220">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="8efd0-221">Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="8efd0-221">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="8efd0-222">applicableDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="8efd0-222">applicableDeviceTypes</span></span>|[<span data-ttu-id="8efd0-223">windowsDeviceType</span><span class="sxs-lookup"><span data-stu-id="8efd0-223">windowsDeviceType</span></span>](../resources/intune-apps-windowsdevicetype.md)|<span data-ttu-id="8efd0-224">Os tipos de dispositivos Windows nos quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="8efd0-224">The Windows device type(s) for which this app can run on.</span></span> <span data-ttu-id="8efd0-225">Os valores possíveis são: `none`, `desktop`, `mobile`, `holographic`, `team`.</span><span class="sxs-lookup"><span data-stu-id="8efd0-225">Possible values are: `none`, `desktop`, `mobile`, `holographic`, `team`.</span></span>|
|<span data-ttu-id="8efd0-226">identityName</span><span class="sxs-lookup"><span data-stu-id="8efd0-226">identityName</span></span>|<span data-ttu-id="8efd0-227">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8efd0-227">String</span></span>|<span data-ttu-id="8efd0-228">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="8efd0-228">The Identity Name.</span></span>|
|<span data-ttu-id="8efd0-229">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="8efd0-229">identityPublisherHash</span></span>|<span data-ttu-id="8efd0-230">String</span><span class="sxs-lookup"><span data-stu-id="8efd0-230">String</span></span>|<span data-ttu-id="8efd0-231">O Hash do Publicador de Identidade.</span><span class="sxs-lookup"><span data-stu-id="8efd0-231">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="8efd0-232">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="8efd0-232">identityResourceIdentifier</span></span>|<span data-ttu-id="8efd0-233">String</span><span class="sxs-lookup"><span data-stu-id="8efd0-233">String</span></span>|<span data-ttu-id="8efd0-234">O Identificador de Recurso da Identidade.</span><span class="sxs-lookup"><span data-stu-id="8efd0-234">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="8efd0-235">isBundle</span><span class="sxs-lookup"><span data-stu-id="8efd0-235">isBundle</span></span>|<span data-ttu-id="8efd0-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="8efd0-236">Boolean</span></span>|<span data-ttu-id="8efd0-237">Se o aplicativo é um pacote ou não.</span><span class="sxs-lookup"><span data-stu-id="8efd0-237">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="8efd0-238">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="8efd0-238">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="8efd0-239">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="8efd0-239">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="8efd0-240">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="8efd0-240">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="8efd0-241">identityVersion</span><span class="sxs-lookup"><span data-stu-id="8efd0-241">identityVersion</span></span>|<span data-ttu-id="8efd0-242">String</span><span class="sxs-lookup"><span data-stu-id="8efd0-242">String</span></span>|<span data-ttu-id="8efd0-243">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="8efd0-243">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="8efd0-244">Resposta</span><span class="sxs-lookup"><span data-stu-id="8efd0-244">Response</span></span>
<span data-ttu-id="8efd0-245">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8efd0-245">If successful, this method returns a `201 Created` response code and a [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8efd0-246">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8efd0-246">Example</span></span>

### <a name="request"></a><span data-ttu-id="8efd0-247">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8efd0-247">Request</span></span>
<span data-ttu-id="8efd0-248">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8efd0-248">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1461

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppX",
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
  "applicableDeviceTypes": "desktop",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
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
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="8efd0-249">Resposta</span><span class="sxs-lookup"><span data-stu-id="8efd0-249">Response</span></span>
<span data-ttu-id="8efd0-p124">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8efd0-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1633

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppX",
  "id": "4bc47eba-7eba-4bc4-ba7e-c44bba7ec44b",
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
  "applicableDeviceTypes": "desktop",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
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
  "identityVersion": "Identity Version value"
}
```





