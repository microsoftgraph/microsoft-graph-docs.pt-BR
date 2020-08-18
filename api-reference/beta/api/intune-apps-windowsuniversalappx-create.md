---
title: Criar windowsUniversalAppX
description: Cria um novo objeto windowsUniversalAppX.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 317667869e49683ccb4b41196fd23be21df2322a
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/18/2020
ms.locfileid: "46791852"
---
# <a name="create-windowsuniversalappx"></a><span data-ttu-id="804d2-103">Criar windowsUniversalAppX</span><span class="sxs-lookup"><span data-stu-id="804d2-103">Create windowsUniversalAppX</span></span>

<span data-ttu-id="804d2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="804d2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="804d2-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="804d2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="804d2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="804d2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="804d2-107">Cria um novo objeto [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="804d2-107">Create a new [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="804d2-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="804d2-108">Prerequisites</span></span>
<span data-ttu-id="804d2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="804d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="804d2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="804d2-111">Permission type</span></span>|<span data-ttu-id="804d2-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="804d2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="804d2-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="804d2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="804d2-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="804d2-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="804d2-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="804d2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="804d2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="804d2-116">Not supported.</span></span>|
|<span data-ttu-id="804d2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="804d2-117">Application</span></span>|<span data-ttu-id="804d2-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="804d2-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="804d2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="804d2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="804d2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="804d2-120">Request headers</span></span>
|<span data-ttu-id="804d2-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="804d2-121">Header</span></span>|<span data-ttu-id="804d2-122">Valor</span><span class="sxs-lookup"><span data-stu-id="804d2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="804d2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="804d2-123">Authorization</span></span>|<span data-ttu-id="804d2-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="804d2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="804d2-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="804d2-125">Accept</span></span>|<span data-ttu-id="804d2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="804d2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="804d2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="804d2-127">Request body</span></span>
<span data-ttu-id="804d2-128">No corpo da solicitação, forneça uma representação JSON do objeto windowsUniversalAppX.</span><span class="sxs-lookup"><span data-stu-id="804d2-128">In the request body, supply a JSON representation for the windowsUniversalAppX object.</span></span>

<span data-ttu-id="804d2-129">A tabela a seguir mostra as propriedades obrigatórias ao criar windowsUniversalAppX.</span><span class="sxs-lookup"><span data-stu-id="804d2-129">The following table shows the properties that are required when you create the windowsUniversalAppX.</span></span>

|<span data-ttu-id="804d2-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="804d2-130">Property</span></span>|<span data-ttu-id="804d2-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="804d2-131">Type</span></span>|<span data-ttu-id="804d2-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="804d2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="804d2-133">id</span><span class="sxs-lookup"><span data-stu-id="804d2-133">id</span></span>|<span data-ttu-id="804d2-134">String</span><span class="sxs-lookup"><span data-stu-id="804d2-134">String</span></span>|<span data-ttu-id="804d2-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="804d2-135">Key of the entity.</span></span> <span data-ttu-id="804d2-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="804d2-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="804d2-137">displayName</span><span class="sxs-lookup"><span data-stu-id="804d2-137">displayName</span></span>|<span data-ttu-id="804d2-138">String</span><span class="sxs-lookup"><span data-stu-id="804d2-138">String</span></span>|<span data-ttu-id="804d2-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="804d2-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="804d2-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="804d2-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="804d2-141">description</span><span class="sxs-lookup"><span data-stu-id="804d2-141">description</span></span>|<span data-ttu-id="804d2-142">String</span><span class="sxs-lookup"><span data-stu-id="804d2-142">String</span></span>|<span data-ttu-id="804d2-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="804d2-143">The description of the app.</span></span> <span data-ttu-id="804d2-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="804d2-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="804d2-145">publicador</span><span class="sxs-lookup"><span data-stu-id="804d2-145">publisher</span></span>|<span data-ttu-id="804d2-146">String</span><span class="sxs-lookup"><span data-stu-id="804d2-146">String</span></span>|<span data-ttu-id="804d2-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="804d2-147">The publisher of the app.</span></span> <span data-ttu-id="804d2-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="804d2-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="804d2-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="804d2-149">largeIcon</span></span>|[<span data-ttu-id="804d2-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="804d2-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="804d2-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="804d2-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="804d2-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="804d2-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="804d2-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="804d2-153">createdDateTime</span></span>|<span data-ttu-id="804d2-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="804d2-154">DateTimeOffset</span></span>|<span data-ttu-id="804d2-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="804d2-155">The date and time the app was created.</span></span> <span data-ttu-id="804d2-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="804d2-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="804d2-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="804d2-157">lastModifiedDateTime</span></span>|<span data-ttu-id="804d2-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="804d2-158">DateTimeOffset</span></span>|<span data-ttu-id="804d2-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="804d2-159">The date and time the app was last modified.</span></span> <span data-ttu-id="804d2-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="804d2-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="804d2-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="804d2-161">isFeatured</span></span>|<span data-ttu-id="804d2-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="804d2-162">Boolean</span></span>|<span data-ttu-id="804d2-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="804d2-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="804d2-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="804d2-164">privacyInformationUrl</span></span>|<span data-ttu-id="804d2-165">String</span><span class="sxs-lookup"><span data-stu-id="804d2-165">String</span></span>|<span data-ttu-id="804d2-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="804d2-166">The privacy statement Url.</span></span> <span data-ttu-id="804d2-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="804d2-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="804d2-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="804d2-168">informationUrl</span></span>|<span data-ttu-id="804d2-169">String</span><span class="sxs-lookup"><span data-stu-id="804d2-169">String</span></span>|<span data-ttu-id="804d2-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="804d2-170">The more information Url.</span></span> <span data-ttu-id="804d2-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="804d2-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="804d2-172">owner</span><span class="sxs-lookup"><span data-stu-id="804d2-172">owner</span></span>|<span data-ttu-id="804d2-173">String</span><span class="sxs-lookup"><span data-stu-id="804d2-173">String</span></span>|<span data-ttu-id="804d2-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="804d2-174">The owner of the app.</span></span> <span data-ttu-id="804d2-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="804d2-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="804d2-176">developer</span><span class="sxs-lookup"><span data-stu-id="804d2-176">developer</span></span>|<span data-ttu-id="804d2-177">String</span><span class="sxs-lookup"><span data-stu-id="804d2-177">String</span></span>|<span data-ttu-id="804d2-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="804d2-178">The developer of the app.</span></span> <span data-ttu-id="804d2-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="804d2-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="804d2-180">notes</span><span class="sxs-lookup"><span data-stu-id="804d2-180">notes</span></span>|<span data-ttu-id="804d2-181">String</span><span class="sxs-lookup"><span data-stu-id="804d2-181">String</span></span>|<span data-ttu-id="804d2-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="804d2-182">Notes for the app.</span></span> <span data-ttu-id="804d2-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="804d2-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="804d2-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="804d2-184">uploadState</span></span>|<span data-ttu-id="804d2-185">Int32</span><span class="sxs-lookup"><span data-stu-id="804d2-185">Int32</span></span>|<span data-ttu-id="804d2-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="804d2-186">The upload state.</span></span> <span data-ttu-id="804d2-187">Os valores possíveis são: 0- `Not Ready` , 1- `Ready` , 2- `Processing` .</span><span class="sxs-lookup"><span data-stu-id="804d2-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="804d2-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="804d2-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="804d2-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="804d2-189">publishingState</span></span>|[<span data-ttu-id="804d2-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="804d2-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="804d2-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="804d2-191">The publishing state for the app.</span></span> <span data-ttu-id="804d2-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="804d2-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="804d2-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="804d2-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="804d2-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="804d2-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="804d2-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="804d2-195">isAssigned</span></span>|<span data-ttu-id="804d2-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="804d2-196">Boolean</span></span>|<span data-ttu-id="804d2-197">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="804d2-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="804d2-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="804d2-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="804d2-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="804d2-199">roleScopeTagIds</span></span>|<span data-ttu-id="804d2-200">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="804d2-200">String collection</span></span>|<span data-ttu-id="804d2-201">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="804d2-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="804d2-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="804d2-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="804d2-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="804d2-203">dependentAppCount</span></span>|<span data-ttu-id="804d2-204">Int32</span><span class="sxs-lookup"><span data-stu-id="804d2-204">Int32</span></span>|<span data-ttu-id="804d2-205">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="804d2-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="804d2-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="804d2-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="804d2-207">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="804d2-207">committedContentVersion</span></span>|<span data-ttu-id="804d2-208">String</span><span class="sxs-lookup"><span data-stu-id="804d2-208">String</span></span>|<span data-ttu-id="804d2-209">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="804d2-209">The internal committed content version.</span></span> <span data-ttu-id="804d2-210">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="804d2-210">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="804d2-211">fileName</span><span class="sxs-lookup"><span data-stu-id="804d2-211">fileName</span></span>|<span data-ttu-id="804d2-212">String</span><span class="sxs-lookup"><span data-stu-id="804d2-212">String</span></span>|<span data-ttu-id="804d2-213">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="804d2-213">The name of the main Lob application file.</span></span> <span data-ttu-id="804d2-214">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="804d2-214">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="804d2-215">size</span><span class="sxs-lookup"><span data-stu-id="804d2-215">size</span></span>|<span data-ttu-id="804d2-216">Int64</span><span class="sxs-lookup"><span data-stu-id="804d2-216">Int64</span></span>|<span data-ttu-id="804d2-217">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="804d2-217">The total size, including all uploaded files.</span></span> <span data-ttu-id="804d2-218">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="804d2-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="804d2-219">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="804d2-219">applicableArchitectures</span></span>|[<span data-ttu-id="804d2-220">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="804d2-220">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="804d2-221">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="804d2-221">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="804d2-222">Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="804d2-222">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="804d2-223">applicableDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="804d2-223">applicableDeviceTypes</span></span>|[<span data-ttu-id="804d2-224">windowsDeviceType</span><span class="sxs-lookup"><span data-stu-id="804d2-224">windowsDeviceType</span></span>](../resources/intune-apps-windowsdevicetype.md)|<span data-ttu-id="804d2-225">Os tipos de dispositivos Windows nos quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="804d2-225">The Windows device type(s) for which this app can run on.</span></span> <span data-ttu-id="804d2-226">Os valores possíveis são: `none`, `desktop`, `mobile`, `holographic`, `team`.</span><span class="sxs-lookup"><span data-stu-id="804d2-226">Possible values are: `none`, `desktop`, `mobile`, `holographic`, `team`.</span></span>|
|<span data-ttu-id="804d2-227">identityName</span><span class="sxs-lookup"><span data-stu-id="804d2-227">identityName</span></span>|<span data-ttu-id="804d2-228">String</span><span class="sxs-lookup"><span data-stu-id="804d2-228">String</span></span>|<span data-ttu-id="804d2-229">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="804d2-229">The Identity Name.</span></span>|
|<span data-ttu-id="804d2-230">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="804d2-230">identityPublisherHash</span></span>|<span data-ttu-id="804d2-231">String</span><span class="sxs-lookup"><span data-stu-id="804d2-231">String</span></span>|<span data-ttu-id="804d2-232">O Hash do Publicador de Identidade.</span><span class="sxs-lookup"><span data-stu-id="804d2-232">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="804d2-233">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="804d2-233">identityResourceIdentifier</span></span>|<span data-ttu-id="804d2-234">String</span><span class="sxs-lookup"><span data-stu-id="804d2-234">String</span></span>|<span data-ttu-id="804d2-235">O Identificador de Recurso da Identidade.</span><span class="sxs-lookup"><span data-stu-id="804d2-235">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="804d2-236">isBundle</span><span class="sxs-lookup"><span data-stu-id="804d2-236">isBundle</span></span>|<span data-ttu-id="804d2-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="804d2-237">Boolean</span></span>|<span data-ttu-id="804d2-238">Se o aplicativo é um pacote ou não.</span><span class="sxs-lookup"><span data-stu-id="804d2-238">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="804d2-239">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="804d2-239">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="804d2-240">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="804d2-240">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="804d2-241">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="804d2-241">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="804d2-242">identityVersion</span><span class="sxs-lookup"><span data-stu-id="804d2-242">identityVersion</span></span>|<span data-ttu-id="804d2-243">String</span><span class="sxs-lookup"><span data-stu-id="804d2-243">String</span></span>|<span data-ttu-id="804d2-244">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="804d2-244">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="804d2-245">Resposta</span><span class="sxs-lookup"><span data-stu-id="804d2-245">Response</span></span>
<span data-ttu-id="804d2-246">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="804d2-246">If successful, this method returns a `201 Created` response code and a [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="804d2-247">Exemplo</span><span class="sxs-lookup"><span data-stu-id="804d2-247">Example</span></span>

### <a name="request"></a><span data-ttu-id="804d2-248">Solicitação</span><span class="sxs-lookup"><span data-stu-id="804d2-248">Request</span></span>
<span data-ttu-id="804d2-249">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="804d2-249">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="804d2-250">Resposta</span><span class="sxs-lookup"><span data-stu-id="804d2-250">Response</span></span>
<span data-ttu-id="804d2-p124">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="804d2-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



