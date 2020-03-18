---
title: Criar windowsPhone81AppX
description: Criar um novo objeto windowsPhone81AppX.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8ed5fe456f13e30030acd6e6858d31fc13aac528
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42760848"
---
# <a name="create-windowsphone81appx"></a><span data-ttu-id="49bc6-103">Criar windowsPhone81AppX</span><span class="sxs-lookup"><span data-stu-id="49bc6-103">Create windowsPhone81AppX</span></span>

> <span data-ttu-id="49bc6-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="49bc6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="49bc6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="49bc6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49bc6-106">Criar um novo objeto [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) .</span><span class="sxs-lookup"><span data-stu-id="49bc6-106">Create a new [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="49bc6-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="49bc6-107">Prerequisites</span></span>
<span data-ttu-id="49bc6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49bc6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49bc6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="49bc6-110">Permission type</span></span>|<span data-ttu-id="49bc6-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="49bc6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49bc6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="49bc6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="49bc6-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49bc6-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="49bc6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="49bc6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49bc6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="49bc6-115">Not supported.</span></span>|
|<span data-ttu-id="49bc6-116">Application</span><span class="sxs-lookup"><span data-stu-id="49bc6-116">Application</span></span>|<span data-ttu-id="49bc6-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49bc6-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="49bc6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="49bc6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="49bc6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="49bc6-119">Request headers</span></span>
|<span data-ttu-id="49bc6-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="49bc6-120">Header</span></span>|<span data-ttu-id="49bc6-121">Valor</span><span class="sxs-lookup"><span data-stu-id="49bc6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="49bc6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="49bc6-122">Authorization</span></span>|<span data-ttu-id="49bc6-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="49bc6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="49bc6-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="49bc6-124">Accept</span></span>|<span data-ttu-id="49bc6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="49bc6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="49bc6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="49bc6-126">Request body</span></span>
<span data-ttu-id="49bc6-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsPhone81AppX.</span><span class="sxs-lookup"><span data-stu-id="49bc6-127">In the request body, supply a JSON representation for the windowsPhone81AppX object.</span></span>

<span data-ttu-id="49bc6-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsPhone81AppX.</span><span class="sxs-lookup"><span data-stu-id="49bc6-128">The following table shows the properties that are required when you create the windowsPhone81AppX.</span></span>

|<span data-ttu-id="49bc6-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="49bc6-129">Property</span></span>|<span data-ttu-id="49bc6-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="49bc6-130">Type</span></span>|<span data-ttu-id="49bc6-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="49bc6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49bc6-132">id</span><span class="sxs-lookup"><span data-stu-id="49bc6-132">id</span></span>|<span data-ttu-id="49bc6-133">String</span><span class="sxs-lookup"><span data-stu-id="49bc6-133">String</span></span>|<span data-ttu-id="49bc6-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="49bc6-134">Key of the entity.</span></span> <span data-ttu-id="49bc6-135">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="49bc6-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="49bc6-136">displayName</span><span class="sxs-lookup"><span data-stu-id="49bc6-136">displayName</span></span>|<span data-ttu-id="49bc6-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="49bc6-137">String</span></span>|<span data-ttu-id="49bc6-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="49bc6-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="49bc6-139">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="49bc6-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="49bc6-140">description</span><span class="sxs-lookup"><span data-stu-id="49bc6-140">description</span></span>|<span data-ttu-id="49bc6-141">String</span><span class="sxs-lookup"><span data-stu-id="49bc6-141">String</span></span>|<span data-ttu-id="49bc6-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="49bc6-142">The description of the app.</span></span> <span data-ttu-id="49bc6-143">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="49bc6-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="49bc6-144">publicador</span><span class="sxs-lookup"><span data-stu-id="49bc6-144">publisher</span></span>|<span data-ttu-id="49bc6-145">String</span><span class="sxs-lookup"><span data-stu-id="49bc6-145">String</span></span>|<span data-ttu-id="49bc6-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="49bc6-146">The publisher of the app.</span></span> <span data-ttu-id="49bc6-147">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="49bc6-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="49bc6-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="49bc6-148">largeIcon</span></span>|[<span data-ttu-id="49bc6-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="49bc6-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="49bc6-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="49bc6-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="49bc6-151">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="49bc6-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="49bc6-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="49bc6-152">createdDateTime</span></span>|<span data-ttu-id="49bc6-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49bc6-153">DateTimeOffset</span></span>|<span data-ttu-id="49bc6-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="49bc6-154">The date and time the app was created.</span></span> <span data-ttu-id="49bc6-155">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="49bc6-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="49bc6-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="49bc6-156">lastModifiedDateTime</span></span>|<span data-ttu-id="49bc6-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49bc6-157">DateTimeOffset</span></span>|<span data-ttu-id="49bc6-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="49bc6-158">The date and time the app was last modified.</span></span> <span data-ttu-id="49bc6-159">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="49bc6-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="49bc6-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="49bc6-160">isFeatured</span></span>|<span data-ttu-id="49bc6-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="49bc6-161">Boolean</span></span>|<span data-ttu-id="49bc6-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="49bc6-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="49bc6-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="49bc6-163">privacyInformationUrl</span></span>|<span data-ttu-id="49bc6-164">String</span><span class="sxs-lookup"><span data-stu-id="49bc6-164">String</span></span>|<span data-ttu-id="49bc6-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="49bc6-165">The privacy statement Url.</span></span> <span data-ttu-id="49bc6-166">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="49bc6-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="49bc6-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="49bc6-167">informationUrl</span></span>|<span data-ttu-id="49bc6-168">String</span><span class="sxs-lookup"><span data-stu-id="49bc6-168">String</span></span>|<span data-ttu-id="49bc6-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="49bc6-169">The more information Url.</span></span> <span data-ttu-id="49bc6-170">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="49bc6-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="49bc6-171">owner</span><span class="sxs-lookup"><span data-stu-id="49bc6-171">owner</span></span>|<span data-ttu-id="49bc6-172">String</span><span class="sxs-lookup"><span data-stu-id="49bc6-172">String</span></span>|<span data-ttu-id="49bc6-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="49bc6-173">The owner of the app.</span></span> <span data-ttu-id="49bc6-174">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="49bc6-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="49bc6-175">developer</span><span class="sxs-lookup"><span data-stu-id="49bc6-175">developer</span></span>|<span data-ttu-id="49bc6-176">String</span><span class="sxs-lookup"><span data-stu-id="49bc6-176">String</span></span>|<span data-ttu-id="49bc6-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="49bc6-177">The developer of the app.</span></span> <span data-ttu-id="49bc6-178">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="49bc6-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="49bc6-179">notes</span><span class="sxs-lookup"><span data-stu-id="49bc6-179">notes</span></span>|<span data-ttu-id="49bc6-180">String</span><span class="sxs-lookup"><span data-stu-id="49bc6-180">String</span></span>|<span data-ttu-id="49bc6-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="49bc6-181">Notes for the app.</span></span> <span data-ttu-id="49bc6-182">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="49bc6-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="49bc6-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="49bc6-183">uploadState</span></span>|<span data-ttu-id="49bc6-184">Int32</span><span class="sxs-lookup"><span data-stu-id="49bc6-184">Int32</span></span>|<span data-ttu-id="49bc6-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="49bc6-185">The upload state.</span></span> <span data-ttu-id="49bc6-186">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="49bc6-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="49bc6-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="49bc6-187">publishingState</span></span>|[<span data-ttu-id="49bc6-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="49bc6-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="49bc6-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="49bc6-189">The publishing state for the app.</span></span> <span data-ttu-id="49bc6-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="49bc6-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="49bc6-191">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="49bc6-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="49bc6-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="49bc6-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="49bc6-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="49bc6-193">isAssigned</span></span>|<span data-ttu-id="49bc6-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="49bc6-194">Boolean</span></span>|<span data-ttu-id="49bc6-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="49bc6-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="49bc6-196">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="49bc6-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="49bc6-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="49bc6-197">roleScopeTagIds</span></span>|<span data-ttu-id="49bc6-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="49bc6-198">String collection</span></span>|<span data-ttu-id="49bc6-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="49bc6-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="49bc6-200">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="49bc6-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="49bc6-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="49bc6-201">dependentAppCount</span></span>|<span data-ttu-id="49bc6-202">Int32</span><span class="sxs-lookup"><span data-stu-id="49bc6-202">Int32</span></span>|<span data-ttu-id="49bc6-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="49bc6-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="49bc6-204">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="49bc6-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="49bc6-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="49bc6-205">committedContentVersion</span></span>|<span data-ttu-id="49bc6-206">String</span><span class="sxs-lookup"><span data-stu-id="49bc6-206">String</span></span>|<span data-ttu-id="49bc6-207">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="49bc6-207">The internal committed content version.</span></span> <span data-ttu-id="49bc6-208">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="49bc6-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="49bc6-209">fileName</span><span class="sxs-lookup"><span data-stu-id="49bc6-209">fileName</span></span>|<span data-ttu-id="49bc6-210">String</span><span class="sxs-lookup"><span data-stu-id="49bc6-210">String</span></span>|<span data-ttu-id="49bc6-211">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="49bc6-211">The name of the main Lob application file.</span></span> <span data-ttu-id="49bc6-212">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="49bc6-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="49bc6-213">size</span><span class="sxs-lookup"><span data-stu-id="49bc6-213">size</span></span>|<span data-ttu-id="49bc6-214">Int64</span><span class="sxs-lookup"><span data-stu-id="49bc6-214">Int64</span></span>|<span data-ttu-id="49bc6-215">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="49bc6-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="49bc6-216">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="49bc6-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="49bc6-217">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="49bc6-217">applicableArchitectures</span></span>|[<span data-ttu-id="49bc6-218">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="49bc6-218">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="49bc6-219">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="49bc6-219">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="49bc6-220">Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="49bc6-220">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="49bc6-221">identityName</span><span class="sxs-lookup"><span data-stu-id="49bc6-221">identityName</span></span>|<span data-ttu-id="49bc6-222">String</span><span class="sxs-lookup"><span data-stu-id="49bc6-222">String</span></span>|<span data-ttu-id="49bc6-223">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="49bc6-223">The Identity Name.</span></span>|
|<span data-ttu-id="49bc6-224">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="49bc6-224">identityPublisherHash</span></span>|<span data-ttu-id="49bc6-225">String</span><span class="sxs-lookup"><span data-stu-id="49bc6-225">String</span></span>|<span data-ttu-id="49bc6-226">O Hash do Publicador de Identidade.</span><span class="sxs-lookup"><span data-stu-id="49bc6-226">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="49bc6-227">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="49bc6-227">identityResourceIdentifier</span></span>|<span data-ttu-id="49bc6-228">String</span><span class="sxs-lookup"><span data-stu-id="49bc6-228">String</span></span>|<span data-ttu-id="49bc6-229">O Identificador de Recurso da Identidade.</span><span class="sxs-lookup"><span data-stu-id="49bc6-229">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="49bc6-230">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="49bc6-230">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="49bc6-231">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="49bc6-231">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="49bc6-232">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="49bc6-232">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="49bc6-233">phoneProductIdentifier</span><span class="sxs-lookup"><span data-stu-id="49bc6-233">phoneProductIdentifier</span></span>|<span data-ttu-id="49bc6-234">String</span><span class="sxs-lookup"><span data-stu-id="49bc6-234">String</span></span>|<span data-ttu-id="49bc6-235">O identificador do produto de telefone.</span><span class="sxs-lookup"><span data-stu-id="49bc6-235">The Phone Product Identifier.</span></span>|
|<span data-ttu-id="49bc6-236">phonePublisherId</span><span class="sxs-lookup"><span data-stu-id="49bc6-236">phonePublisherId</span></span>|<span data-ttu-id="49bc6-237">String</span><span class="sxs-lookup"><span data-stu-id="49bc6-237">String</span></span>|<span data-ttu-id="49bc6-238">A ID do editor do telefone.</span><span class="sxs-lookup"><span data-stu-id="49bc6-238">The Phone Publisher Id.</span></span>|
|<span data-ttu-id="49bc6-239">identityVersion</span><span class="sxs-lookup"><span data-stu-id="49bc6-239">identityVersion</span></span>|<span data-ttu-id="49bc6-240">String</span><span class="sxs-lookup"><span data-stu-id="49bc6-240">String</span></span>|<span data-ttu-id="49bc6-241">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="49bc6-241">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="49bc6-242">Resposta</span><span class="sxs-lookup"><span data-stu-id="49bc6-242">Response</span></span>
<span data-ttu-id="49bc6-243">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="49bc6-243">If successful, this method returns a `201 Created` response code and a [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49bc6-244">Exemplo</span><span class="sxs-lookup"><span data-stu-id="49bc6-244">Example</span></span>

### <a name="request"></a><span data-ttu-id="49bc6-245">Solicitação</span><span class="sxs-lookup"><span data-stu-id="49bc6-245">Request</span></span>
<span data-ttu-id="49bc6-246">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="49bc6-246">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1513

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
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="49bc6-247">Resposta</span><span class="sxs-lookup"><span data-stu-id="49bc6-247">Response</span></span>
<span data-ttu-id="49bc6-p123">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="49bc6-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1685

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
  "identityVersion": "Identity Version value"
}
```




