---
title: Criar windowsAppX
description: Criar um novo objeto windowsAppX.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 40367ab7d5a8d546694f24a8bf75cb7c0920757f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36328722"
---
# <a name="create-windowsappx"></a><span data-ttu-id="9e3ac-103">Criar windowsAppX</span><span class="sxs-lookup"><span data-stu-id="9e3ac-103">Create windowsAppX</span></span>

> <span data-ttu-id="9e3ac-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9e3ac-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9e3ac-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9e3ac-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e3ac-106">Criar um novo objeto [windowsAppX](../resources/intune-apps-windowsappx.md) .</span><span class="sxs-lookup"><span data-stu-id="9e3ac-106">Create a new [windowsAppX](../resources/intune-apps-windowsappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9e3ac-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9e3ac-107">Prerequisites</span></span>
<span data-ttu-id="9e3ac-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e3ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e3ac-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9e3ac-110">Permission type</span></span>|<span data-ttu-id="9e3ac-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9e3ac-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9e3ac-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9e3ac-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9e3ac-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e3ac-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9e3ac-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9e3ac-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9e3ac-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9e3ac-115">Not supported.</span></span>|
|<span data-ttu-id="9e3ac-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9e3ac-116">Application</span></span>|<span data-ttu-id="9e3ac-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e3ac-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9e3ac-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9e3ac-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="9e3ac-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9e3ac-119">Request headers</span></span>
|<span data-ttu-id="9e3ac-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9e3ac-120">Header</span></span>|<span data-ttu-id="9e3ac-121">Valor</span><span class="sxs-lookup"><span data-stu-id="9e3ac-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9e3ac-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9e3ac-122">Authorization</span></span>|<span data-ttu-id="9e3ac-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9e3ac-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9e3ac-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9e3ac-124">Accept</span></span>|<span data-ttu-id="9e3ac-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9e3ac-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e3ac-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9e3ac-126">Request body</span></span>
<span data-ttu-id="9e3ac-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsAppX.</span><span class="sxs-lookup"><span data-stu-id="9e3ac-127">In the request body, supply a JSON representation for the windowsAppX object.</span></span>

<span data-ttu-id="9e3ac-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsAppX.</span><span class="sxs-lookup"><span data-stu-id="9e3ac-128">The following table shows the properties that are required when you create the windowsAppX.</span></span>

|<span data-ttu-id="9e3ac-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9e3ac-129">Property</span></span>|<span data-ttu-id="9e3ac-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="9e3ac-130">Type</span></span>|<span data-ttu-id="9e3ac-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e3ac-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e3ac-132">id</span><span class="sxs-lookup"><span data-stu-id="9e3ac-132">id</span></span>|<span data-ttu-id="9e3ac-133">String</span><span class="sxs-lookup"><span data-stu-id="9e3ac-133">String</span></span>|<span data-ttu-id="9e3ac-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9e3ac-134">Key of the entity.</span></span> <span data-ttu-id="9e3ac-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9e3ac-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9e3ac-136">displayName</span><span class="sxs-lookup"><span data-stu-id="9e3ac-136">displayName</span></span>|<span data-ttu-id="9e3ac-137">String</span><span class="sxs-lookup"><span data-stu-id="9e3ac-137">String</span></span>|<span data-ttu-id="9e3ac-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="9e3ac-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="9e3ac-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9e3ac-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9e3ac-140">descrição</span><span class="sxs-lookup"><span data-stu-id="9e3ac-140">description</span></span>|<span data-ttu-id="9e3ac-141">String</span><span class="sxs-lookup"><span data-stu-id="9e3ac-141">String</span></span>|<span data-ttu-id="9e3ac-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9e3ac-142">The description of the app.</span></span> <span data-ttu-id="9e3ac-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9e3ac-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9e3ac-144">publicador</span><span class="sxs-lookup"><span data-stu-id="9e3ac-144">publisher</span></span>|<span data-ttu-id="9e3ac-145">String</span><span class="sxs-lookup"><span data-stu-id="9e3ac-145">String</span></span>|<span data-ttu-id="9e3ac-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9e3ac-146">The publisher of the app.</span></span> <span data-ttu-id="9e3ac-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9e3ac-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9e3ac-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="9e3ac-148">largeIcon</span></span>|[<span data-ttu-id="9e3ac-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="9e3ac-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="9e3ac-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="9e3ac-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="9e3ac-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9e3ac-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9e3ac-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9e3ac-152">createdDateTime</span></span>|<span data-ttu-id="9e3ac-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e3ac-153">DateTimeOffset</span></span>|<span data-ttu-id="9e3ac-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9e3ac-154">The date and time the app was created.</span></span> <span data-ttu-id="9e3ac-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9e3ac-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9e3ac-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9e3ac-156">lastModifiedDateTime</span></span>|<span data-ttu-id="9e3ac-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e3ac-157">DateTimeOffset</span></span>|<span data-ttu-id="9e3ac-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="9e3ac-158">The date and time the app was last modified.</span></span> <span data-ttu-id="9e3ac-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9e3ac-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9e3ac-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="9e3ac-160">isFeatured</span></span>|<span data-ttu-id="9e3ac-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e3ac-161">Boolean</span></span>|<span data-ttu-id="9e3ac-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9e3ac-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9e3ac-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="9e3ac-163">privacyInformationUrl</span></span>|<span data-ttu-id="9e3ac-164">String</span><span class="sxs-lookup"><span data-stu-id="9e3ac-164">String</span></span>|<span data-ttu-id="9e3ac-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="9e3ac-165">The privacy statement Url.</span></span> <span data-ttu-id="9e3ac-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9e3ac-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9e3ac-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="9e3ac-167">informationUrl</span></span>|<span data-ttu-id="9e3ac-168">String</span><span class="sxs-lookup"><span data-stu-id="9e3ac-168">String</span></span>|<span data-ttu-id="9e3ac-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="9e3ac-169">The more information Url.</span></span> <span data-ttu-id="9e3ac-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9e3ac-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9e3ac-171">owner</span><span class="sxs-lookup"><span data-stu-id="9e3ac-171">owner</span></span>|<span data-ttu-id="9e3ac-172">String</span><span class="sxs-lookup"><span data-stu-id="9e3ac-172">String</span></span>|<span data-ttu-id="9e3ac-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="9e3ac-173">The owner of the app.</span></span> <span data-ttu-id="9e3ac-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9e3ac-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9e3ac-175">developer</span><span class="sxs-lookup"><span data-stu-id="9e3ac-175">developer</span></span>|<span data-ttu-id="9e3ac-176">String</span><span class="sxs-lookup"><span data-stu-id="9e3ac-176">String</span></span>|<span data-ttu-id="9e3ac-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9e3ac-177">The developer of the app.</span></span> <span data-ttu-id="9e3ac-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9e3ac-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9e3ac-179">notes</span><span class="sxs-lookup"><span data-stu-id="9e3ac-179">notes</span></span>|<span data-ttu-id="9e3ac-180">String</span><span class="sxs-lookup"><span data-stu-id="9e3ac-180">String</span></span>|<span data-ttu-id="9e3ac-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9e3ac-181">Notes for the app.</span></span> <span data-ttu-id="9e3ac-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9e3ac-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9e3ac-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="9e3ac-183">uploadState</span></span>|<span data-ttu-id="9e3ac-184">Int32</span><span class="sxs-lookup"><span data-stu-id="9e3ac-184">Int32</span></span>|<span data-ttu-id="9e3ac-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="9e3ac-185">The upload state.</span></span> <span data-ttu-id="9e3ac-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9e3ac-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9e3ac-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="9e3ac-187">publishingState</span></span>|[<span data-ttu-id="9e3ac-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="9e3ac-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="9e3ac-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9e3ac-189">The publishing state for the app.</span></span> <span data-ttu-id="9e3ac-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="9e3ac-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="9e3ac-191">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9e3ac-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="9e3ac-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="9e3ac-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="9e3ac-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="9e3ac-193">isAssigned</span></span>|<span data-ttu-id="9e3ac-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e3ac-194">Boolean</span></span>|<span data-ttu-id="9e3ac-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="9e3ac-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="9e3ac-196">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9e3ac-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9e3ac-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9e3ac-197">roleScopeTagIds</span></span>|<span data-ttu-id="9e3ac-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9e3ac-198">String collection</span></span>|<span data-ttu-id="9e3ac-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="9e3ac-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="9e3ac-200">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9e3ac-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9e3ac-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="9e3ac-201">dependentAppCount</span></span>|<span data-ttu-id="9e3ac-202">Int32</span><span class="sxs-lookup"><span data-stu-id="9e3ac-202">Int32</span></span>|<span data-ttu-id="9e3ac-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="9e3ac-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="9e3ac-204">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9e3ac-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9e3ac-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="9e3ac-205">committedContentVersion</span></span>|<span data-ttu-id="9e3ac-206">String</span><span class="sxs-lookup"><span data-stu-id="9e3ac-206">String</span></span>|<span data-ttu-id="9e3ac-207">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="9e3ac-207">The internal committed content version.</span></span> <span data-ttu-id="9e3ac-208">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="9e3ac-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="9e3ac-209">fileName</span><span class="sxs-lookup"><span data-stu-id="9e3ac-209">fileName</span></span>|<span data-ttu-id="9e3ac-210">String</span><span class="sxs-lookup"><span data-stu-id="9e3ac-210">String</span></span>|<span data-ttu-id="9e3ac-211">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="9e3ac-211">The name of the main Lob application file.</span></span> <span data-ttu-id="9e3ac-212">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="9e3ac-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="9e3ac-213">size</span><span class="sxs-lookup"><span data-stu-id="9e3ac-213">size</span></span>|<span data-ttu-id="9e3ac-214">Int64</span><span class="sxs-lookup"><span data-stu-id="9e3ac-214">Int64</span></span>|<span data-ttu-id="9e3ac-215">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="9e3ac-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="9e3ac-216">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="9e3ac-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="9e3ac-217">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="9e3ac-217">applicableArchitectures</span></span>|[<span data-ttu-id="9e3ac-218">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="9e3ac-218">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="9e3ac-219">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="9e3ac-219">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="9e3ac-220">Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="9e3ac-220">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="9e3ac-221">identityName</span><span class="sxs-lookup"><span data-stu-id="9e3ac-221">identityName</span></span>|<span data-ttu-id="9e3ac-222">String</span><span class="sxs-lookup"><span data-stu-id="9e3ac-222">String</span></span>|<span data-ttu-id="9e3ac-223">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="9e3ac-223">The Identity Name.</span></span>|
|<span data-ttu-id="9e3ac-224">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="9e3ac-224">identityPublisherHash</span></span>|<span data-ttu-id="9e3ac-225">String</span><span class="sxs-lookup"><span data-stu-id="9e3ac-225">String</span></span>|<span data-ttu-id="9e3ac-226">O Hash do Publicador de Identidade.</span><span class="sxs-lookup"><span data-stu-id="9e3ac-226">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="9e3ac-227">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="9e3ac-227">identityResourceIdentifier</span></span>|<span data-ttu-id="9e3ac-228">String</span><span class="sxs-lookup"><span data-stu-id="9e3ac-228">String</span></span>|<span data-ttu-id="9e3ac-229">O Identificador de Recurso da Identidade.</span><span class="sxs-lookup"><span data-stu-id="9e3ac-229">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="9e3ac-230">isBundle</span><span class="sxs-lookup"><span data-stu-id="9e3ac-230">isBundle</span></span>|<span data-ttu-id="9e3ac-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e3ac-231">Boolean</span></span>|<span data-ttu-id="9e3ac-232">Se o aplicativo é um pacote ou não.</span><span class="sxs-lookup"><span data-stu-id="9e3ac-232">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="9e3ac-233">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="9e3ac-233">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="9e3ac-234">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="9e3ac-234">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="9e3ac-235">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="9e3ac-235">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="9e3ac-236">identityVersion</span><span class="sxs-lookup"><span data-stu-id="9e3ac-236">identityVersion</span></span>|<span data-ttu-id="9e3ac-237">String</span><span class="sxs-lookup"><span data-stu-id="9e3ac-237">String</span></span>|<span data-ttu-id="9e3ac-238">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="9e3ac-238">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="9e3ac-239">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e3ac-239">Response</span></span>
<span data-ttu-id="9e3ac-240">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsAppX](../resources/intune-apps-windowsappx.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9e3ac-240">If successful, this method returns a `201 Created` response code and a [windowsAppX](../resources/intune-apps-windowsappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e3ac-241">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9e3ac-241">Example</span></span>

### <a name="request"></a><span data-ttu-id="9e3ac-242">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9e3ac-242">Request</span></span>
<span data-ttu-id="9e3ac-243">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9e3ac-243">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9e3ac-244">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e3ac-244">Response</span></span>
<span data-ttu-id="9e3ac-p123">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9e3ac-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






