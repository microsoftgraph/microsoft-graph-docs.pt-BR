---
title: Criar windowsAppX
description: Criar um novo objeto windowsAppX.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 957776f9617003f333d05fed7d310fd8258298a3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35960162"
---
# <a name="create-windowsappx"></a><span data-ttu-id="a9cdb-103">Criar windowsAppX</span><span class="sxs-lookup"><span data-stu-id="a9cdb-103">Create windowsAppX</span></span>

> <span data-ttu-id="a9cdb-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a9cdb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a9cdb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a9cdb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9cdb-106">Criar um novo objeto [windowsAppX](../resources/intune-apps-windowsappx.md) .</span><span class="sxs-lookup"><span data-stu-id="a9cdb-106">Create a new [windowsAppX](../resources/intune-apps-windowsappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a9cdb-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a9cdb-107">Prerequisites</span></span>
<span data-ttu-id="a9cdb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9cdb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9cdb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a9cdb-110">Permission type</span></span>|<span data-ttu-id="a9cdb-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a9cdb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a9cdb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a9cdb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a9cdb-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9cdb-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a9cdb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a9cdb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9cdb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9cdb-115">Not supported.</span></span>|
|<span data-ttu-id="a9cdb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a9cdb-116">Application</span></span>|<span data-ttu-id="a9cdb-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9cdb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9cdb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a9cdb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="a9cdb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a9cdb-119">Request headers</span></span>
|<span data-ttu-id="a9cdb-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a9cdb-120">Header</span></span>|<span data-ttu-id="a9cdb-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a9cdb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a9cdb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a9cdb-122">Authorization</span></span>|<span data-ttu-id="a9cdb-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a9cdb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a9cdb-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a9cdb-124">Accept</span></span>|<span data-ttu-id="a9cdb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a9cdb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9cdb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a9cdb-126">Request body</span></span>
<span data-ttu-id="a9cdb-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsAppX.</span><span class="sxs-lookup"><span data-stu-id="a9cdb-127">In the request body, supply a JSON representation for the windowsAppX object.</span></span>

<span data-ttu-id="a9cdb-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsAppX.</span><span class="sxs-lookup"><span data-stu-id="a9cdb-128">The following table shows the properties that are required when you create the windowsAppX.</span></span>

|<span data-ttu-id="a9cdb-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a9cdb-129">Property</span></span>|<span data-ttu-id="a9cdb-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a9cdb-130">Type</span></span>|<span data-ttu-id="a9cdb-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9cdb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9cdb-132">id</span><span class="sxs-lookup"><span data-stu-id="a9cdb-132">id</span></span>|<span data-ttu-id="a9cdb-133">String</span><span class="sxs-lookup"><span data-stu-id="a9cdb-133">String</span></span>|<span data-ttu-id="a9cdb-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a9cdb-134">Key of the entity.</span></span> <span data-ttu-id="a9cdb-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a9cdb-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a9cdb-136">displayName</span><span class="sxs-lookup"><span data-stu-id="a9cdb-136">displayName</span></span>|<span data-ttu-id="a9cdb-137">String</span><span class="sxs-lookup"><span data-stu-id="a9cdb-137">String</span></span>|<span data-ttu-id="a9cdb-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="a9cdb-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="a9cdb-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a9cdb-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a9cdb-140">descrição</span><span class="sxs-lookup"><span data-stu-id="a9cdb-140">description</span></span>|<span data-ttu-id="a9cdb-141">String</span><span class="sxs-lookup"><span data-stu-id="a9cdb-141">String</span></span>|<span data-ttu-id="a9cdb-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a9cdb-142">The description of the app.</span></span> <span data-ttu-id="a9cdb-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a9cdb-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a9cdb-144">publicador</span><span class="sxs-lookup"><span data-stu-id="a9cdb-144">publisher</span></span>|<span data-ttu-id="a9cdb-145">String</span><span class="sxs-lookup"><span data-stu-id="a9cdb-145">String</span></span>|<span data-ttu-id="a9cdb-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a9cdb-146">The publisher of the app.</span></span> <span data-ttu-id="a9cdb-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a9cdb-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a9cdb-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="a9cdb-148">largeIcon</span></span>|[<span data-ttu-id="a9cdb-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="a9cdb-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="a9cdb-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="a9cdb-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="a9cdb-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a9cdb-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a9cdb-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a9cdb-152">createdDateTime</span></span>|<span data-ttu-id="a9cdb-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9cdb-153">DateTimeOffset</span></span>|<span data-ttu-id="a9cdb-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a9cdb-154">The date and time the app was created.</span></span> <span data-ttu-id="a9cdb-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a9cdb-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a9cdb-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a9cdb-156">lastModifiedDateTime</span></span>|<span data-ttu-id="a9cdb-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9cdb-157">DateTimeOffset</span></span>|<span data-ttu-id="a9cdb-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="a9cdb-158">The date and time the app was last modified.</span></span> <span data-ttu-id="a9cdb-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a9cdb-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a9cdb-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="a9cdb-160">isFeatured</span></span>|<span data-ttu-id="a9cdb-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9cdb-161">Boolean</span></span>|<span data-ttu-id="a9cdb-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a9cdb-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a9cdb-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="a9cdb-163">privacyInformationUrl</span></span>|<span data-ttu-id="a9cdb-164">String</span><span class="sxs-lookup"><span data-stu-id="a9cdb-164">String</span></span>|<span data-ttu-id="a9cdb-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="a9cdb-165">The privacy statement Url.</span></span> <span data-ttu-id="a9cdb-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a9cdb-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a9cdb-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="a9cdb-167">informationUrl</span></span>|<span data-ttu-id="a9cdb-168">String</span><span class="sxs-lookup"><span data-stu-id="a9cdb-168">String</span></span>|<span data-ttu-id="a9cdb-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="a9cdb-169">The more information Url.</span></span> <span data-ttu-id="a9cdb-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a9cdb-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a9cdb-171">owner</span><span class="sxs-lookup"><span data-stu-id="a9cdb-171">owner</span></span>|<span data-ttu-id="a9cdb-172">String</span><span class="sxs-lookup"><span data-stu-id="a9cdb-172">String</span></span>|<span data-ttu-id="a9cdb-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="a9cdb-173">The owner of the app.</span></span> <span data-ttu-id="a9cdb-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a9cdb-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a9cdb-175">developer</span><span class="sxs-lookup"><span data-stu-id="a9cdb-175">developer</span></span>|<span data-ttu-id="a9cdb-176">String</span><span class="sxs-lookup"><span data-stu-id="a9cdb-176">String</span></span>|<span data-ttu-id="a9cdb-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a9cdb-177">The developer of the app.</span></span> <span data-ttu-id="a9cdb-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a9cdb-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a9cdb-179">notes</span><span class="sxs-lookup"><span data-stu-id="a9cdb-179">notes</span></span>|<span data-ttu-id="a9cdb-180">String</span><span class="sxs-lookup"><span data-stu-id="a9cdb-180">String</span></span>|<span data-ttu-id="a9cdb-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a9cdb-181">Notes for the app.</span></span> <span data-ttu-id="a9cdb-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a9cdb-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a9cdb-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="a9cdb-183">uploadState</span></span>|<span data-ttu-id="a9cdb-184">Int32</span><span class="sxs-lookup"><span data-stu-id="a9cdb-184">Int32</span></span>|<span data-ttu-id="a9cdb-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="a9cdb-185">The upload state.</span></span> <span data-ttu-id="a9cdb-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a9cdb-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a9cdb-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="a9cdb-187">publishingState</span></span>|[<span data-ttu-id="a9cdb-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="a9cdb-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="a9cdb-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a9cdb-189">The publishing state for the app.</span></span> <span data-ttu-id="a9cdb-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="a9cdb-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="a9cdb-191">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a9cdb-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="a9cdb-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="a9cdb-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="a9cdb-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="a9cdb-193">isAssigned</span></span>|<span data-ttu-id="a9cdb-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9cdb-194">Boolean</span></span>|<span data-ttu-id="a9cdb-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="a9cdb-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="a9cdb-196">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a9cdb-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a9cdb-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a9cdb-197">roleScopeTagIds</span></span>|<span data-ttu-id="a9cdb-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a9cdb-198">String collection</span></span>|<span data-ttu-id="a9cdb-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="a9cdb-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="a9cdb-200">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a9cdb-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a9cdb-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="a9cdb-201">dependentAppCount</span></span>|<span data-ttu-id="a9cdb-202">Int32</span><span class="sxs-lookup"><span data-stu-id="a9cdb-202">Int32</span></span>|<span data-ttu-id="a9cdb-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="a9cdb-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="a9cdb-204">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a9cdb-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a9cdb-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="a9cdb-205">committedContentVersion</span></span>|<span data-ttu-id="a9cdb-206">String</span><span class="sxs-lookup"><span data-stu-id="a9cdb-206">String</span></span>|<span data-ttu-id="a9cdb-207">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="a9cdb-207">The internal committed content version.</span></span> <span data-ttu-id="a9cdb-208">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="a9cdb-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="a9cdb-209">fileName</span><span class="sxs-lookup"><span data-stu-id="a9cdb-209">fileName</span></span>|<span data-ttu-id="a9cdb-210">String</span><span class="sxs-lookup"><span data-stu-id="a9cdb-210">String</span></span>|<span data-ttu-id="a9cdb-211">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="a9cdb-211">The name of the main Lob application file.</span></span> <span data-ttu-id="a9cdb-212">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="a9cdb-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="a9cdb-213">size</span><span class="sxs-lookup"><span data-stu-id="a9cdb-213">size</span></span>|<span data-ttu-id="a9cdb-214">Int64</span><span class="sxs-lookup"><span data-stu-id="a9cdb-214">Int64</span></span>|<span data-ttu-id="a9cdb-215">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="a9cdb-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="a9cdb-216">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="a9cdb-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="a9cdb-217">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="a9cdb-217">applicableArchitectures</span></span>|[<span data-ttu-id="a9cdb-218">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="a9cdb-218">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="a9cdb-219">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="a9cdb-219">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="a9cdb-220">Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="a9cdb-220">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="a9cdb-221">identityName</span><span class="sxs-lookup"><span data-stu-id="a9cdb-221">identityName</span></span>|<span data-ttu-id="a9cdb-222">String</span><span class="sxs-lookup"><span data-stu-id="a9cdb-222">String</span></span>|<span data-ttu-id="a9cdb-223">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="a9cdb-223">The Identity Name.</span></span>|
|<span data-ttu-id="a9cdb-224">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="a9cdb-224">identityPublisherHash</span></span>|<span data-ttu-id="a9cdb-225">String</span><span class="sxs-lookup"><span data-stu-id="a9cdb-225">String</span></span>|<span data-ttu-id="a9cdb-226">O Hash do Publicador de Identidade.</span><span class="sxs-lookup"><span data-stu-id="a9cdb-226">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="a9cdb-227">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="a9cdb-227">identityResourceIdentifier</span></span>|<span data-ttu-id="a9cdb-228">String</span><span class="sxs-lookup"><span data-stu-id="a9cdb-228">String</span></span>|<span data-ttu-id="a9cdb-229">O Identificador de Recurso da Identidade.</span><span class="sxs-lookup"><span data-stu-id="a9cdb-229">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="a9cdb-230">isBundle</span><span class="sxs-lookup"><span data-stu-id="a9cdb-230">isBundle</span></span>|<span data-ttu-id="a9cdb-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9cdb-231">Boolean</span></span>|<span data-ttu-id="a9cdb-232">Se o aplicativo é um pacote ou não.</span><span class="sxs-lookup"><span data-stu-id="a9cdb-232">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="a9cdb-233">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="a9cdb-233">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="a9cdb-234">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="a9cdb-234">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="a9cdb-235">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="a9cdb-235">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="a9cdb-236">identityVersion</span><span class="sxs-lookup"><span data-stu-id="a9cdb-236">identityVersion</span></span>|<span data-ttu-id="a9cdb-237">String</span><span class="sxs-lookup"><span data-stu-id="a9cdb-237">String</span></span>|<span data-ttu-id="a9cdb-238">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="a9cdb-238">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="a9cdb-239">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9cdb-239">Response</span></span>
<span data-ttu-id="a9cdb-240">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsAppX](../resources/intune-apps-windowsappx.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a9cdb-240">If successful, this method returns a `201 Created` response code and a [windowsAppX](../resources/intune-apps-windowsappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9cdb-241">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a9cdb-241">Example</span></span>

### <a name="request"></a><span data-ttu-id="a9cdb-242">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9cdb-242">Request</span></span>
<span data-ttu-id="a9cdb-243">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a9cdb-243">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1413

{
  "@odata.type": "#microsoft.graph.windowsAppX",
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

### <a name="response"></a><span data-ttu-id="a9cdb-244">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9cdb-244">Response</span></span>
<span data-ttu-id="a9cdb-p123">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a9cdb-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1585

{
  "@odata.type": "#microsoft.graph.windowsAppX",
  "id": "b5179a93-9a93-b517-939a-17b5939a17b5",
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





