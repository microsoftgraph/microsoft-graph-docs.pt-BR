---
title: Criar windowsPhone81AppX
description: Criar um novo objeto windowsPhone81AppX.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 20b73f1e7702400b98ca5638fc8e6522c5cbb668
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37535034"
---
# <a name="create-windowsphone81appx"></a><span data-ttu-id="59f40-103">Criar windowsPhone81AppX</span><span class="sxs-lookup"><span data-stu-id="59f40-103">Create windowsPhone81AppX</span></span>

> <span data-ttu-id="59f40-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="59f40-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="59f40-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="59f40-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="59f40-106">Criar um novo objeto [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) .</span><span class="sxs-lookup"><span data-stu-id="59f40-106">Create a new [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="59f40-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="59f40-107">Prerequisites</span></span>
<span data-ttu-id="59f40-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59f40-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59f40-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="59f40-110">Permission type</span></span>|<span data-ttu-id="59f40-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="59f40-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="59f40-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="59f40-112">Delegated (work or school account)</span></span>|<span data-ttu-id="59f40-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59f40-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="59f40-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="59f40-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="59f40-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="59f40-115">Not supported.</span></span>|
|<span data-ttu-id="59f40-116">Application</span><span class="sxs-lookup"><span data-stu-id="59f40-116">Application</span></span>|<span data-ttu-id="59f40-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59f40-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="59f40-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="59f40-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="59f40-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="59f40-119">Request headers</span></span>
|<span data-ttu-id="59f40-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="59f40-120">Header</span></span>|<span data-ttu-id="59f40-121">Valor</span><span class="sxs-lookup"><span data-stu-id="59f40-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="59f40-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="59f40-122">Authorization</span></span>|<span data-ttu-id="59f40-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59f40-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="59f40-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="59f40-124">Accept</span></span>|<span data-ttu-id="59f40-125">application/json</span><span class="sxs-lookup"><span data-stu-id="59f40-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="59f40-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="59f40-126">Request body</span></span>
<span data-ttu-id="59f40-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsPhone81AppX.</span><span class="sxs-lookup"><span data-stu-id="59f40-127">In the request body, supply a JSON representation for the windowsPhone81AppX object.</span></span>

<span data-ttu-id="59f40-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsPhone81AppX.</span><span class="sxs-lookup"><span data-stu-id="59f40-128">The following table shows the properties that are required when you create the windowsPhone81AppX.</span></span>

|<span data-ttu-id="59f40-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="59f40-129">Property</span></span>|<span data-ttu-id="59f40-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="59f40-130">Type</span></span>|<span data-ttu-id="59f40-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="59f40-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59f40-132">id</span><span class="sxs-lookup"><span data-stu-id="59f40-132">id</span></span>|<span data-ttu-id="59f40-133">String</span><span class="sxs-lookup"><span data-stu-id="59f40-133">String</span></span>|<span data-ttu-id="59f40-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="59f40-134">Key of the entity.</span></span> <span data-ttu-id="59f40-135">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="59f40-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="59f40-136">displayName</span><span class="sxs-lookup"><span data-stu-id="59f40-136">displayName</span></span>|<span data-ttu-id="59f40-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59f40-137">String</span></span>|<span data-ttu-id="59f40-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="59f40-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="59f40-139">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="59f40-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="59f40-140">description</span><span class="sxs-lookup"><span data-stu-id="59f40-140">description</span></span>|<span data-ttu-id="59f40-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59f40-141">String</span></span>|<span data-ttu-id="59f40-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="59f40-142">The description of the app.</span></span> <span data-ttu-id="59f40-143">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="59f40-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="59f40-144">publicador</span><span class="sxs-lookup"><span data-stu-id="59f40-144">publisher</span></span>|<span data-ttu-id="59f40-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59f40-145">String</span></span>|<span data-ttu-id="59f40-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="59f40-146">The publisher of the app.</span></span> <span data-ttu-id="59f40-147">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="59f40-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="59f40-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="59f40-148">largeIcon</span></span>|[<span data-ttu-id="59f40-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="59f40-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="59f40-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="59f40-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="59f40-151">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="59f40-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="59f40-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="59f40-152">createdDateTime</span></span>|<span data-ttu-id="59f40-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59f40-153">DateTimeOffset</span></span>|<span data-ttu-id="59f40-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="59f40-154">The date and time the app was created.</span></span> <span data-ttu-id="59f40-155">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="59f40-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="59f40-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="59f40-156">lastModifiedDateTime</span></span>|<span data-ttu-id="59f40-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59f40-157">DateTimeOffset</span></span>|<span data-ttu-id="59f40-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="59f40-158">The date and time the app was last modified.</span></span> <span data-ttu-id="59f40-159">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="59f40-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="59f40-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="59f40-160">isFeatured</span></span>|<span data-ttu-id="59f40-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="59f40-161">Boolean</span></span>|<span data-ttu-id="59f40-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="59f40-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="59f40-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="59f40-163">privacyInformationUrl</span></span>|<span data-ttu-id="59f40-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59f40-164">String</span></span>|<span data-ttu-id="59f40-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="59f40-165">The privacy statement Url.</span></span> <span data-ttu-id="59f40-166">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="59f40-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="59f40-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="59f40-167">informationUrl</span></span>|<span data-ttu-id="59f40-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59f40-168">String</span></span>|<span data-ttu-id="59f40-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="59f40-169">The more information Url.</span></span> <span data-ttu-id="59f40-170">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="59f40-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="59f40-171">owner</span><span class="sxs-lookup"><span data-stu-id="59f40-171">owner</span></span>|<span data-ttu-id="59f40-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59f40-172">String</span></span>|<span data-ttu-id="59f40-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="59f40-173">The owner of the app.</span></span> <span data-ttu-id="59f40-174">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="59f40-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="59f40-175">developer</span><span class="sxs-lookup"><span data-stu-id="59f40-175">developer</span></span>|<span data-ttu-id="59f40-176">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59f40-176">String</span></span>|<span data-ttu-id="59f40-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="59f40-177">The developer of the app.</span></span> <span data-ttu-id="59f40-178">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="59f40-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="59f40-179">notes</span><span class="sxs-lookup"><span data-stu-id="59f40-179">notes</span></span>|<span data-ttu-id="59f40-180">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59f40-180">String</span></span>|<span data-ttu-id="59f40-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="59f40-181">Notes for the app.</span></span> <span data-ttu-id="59f40-182">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="59f40-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="59f40-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="59f40-183">uploadState</span></span>|<span data-ttu-id="59f40-184">Int32</span><span class="sxs-lookup"><span data-stu-id="59f40-184">Int32</span></span>|<span data-ttu-id="59f40-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="59f40-185">The upload state.</span></span> <span data-ttu-id="59f40-186">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="59f40-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="59f40-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="59f40-187">publishingState</span></span>|[<span data-ttu-id="59f40-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="59f40-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="59f40-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="59f40-189">The publishing state for the app.</span></span> <span data-ttu-id="59f40-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="59f40-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="59f40-191">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="59f40-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="59f40-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="59f40-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="59f40-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="59f40-193">isAssigned</span></span>|<span data-ttu-id="59f40-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="59f40-194">Boolean</span></span>|<span data-ttu-id="59f40-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="59f40-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="59f40-196">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="59f40-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="59f40-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="59f40-197">roleScopeTagIds</span></span>|<span data-ttu-id="59f40-198">String collection</span><span class="sxs-lookup"><span data-stu-id="59f40-198">String collection</span></span>|<span data-ttu-id="59f40-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="59f40-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="59f40-200">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="59f40-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="59f40-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="59f40-201">dependentAppCount</span></span>|<span data-ttu-id="59f40-202">Int32</span><span class="sxs-lookup"><span data-stu-id="59f40-202">Int32</span></span>|<span data-ttu-id="59f40-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="59f40-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="59f40-204">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="59f40-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="59f40-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="59f40-205">committedContentVersion</span></span>|<span data-ttu-id="59f40-206">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59f40-206">String</span></span>|<span data-ttu-id="59f40-207">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="59f40-207">The internal committed content version.</span></span> <span data-ttu-id="59f40-208">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="59f40-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="59f40-209">fileName</span><span class="sxs-lookup"><span data-stu-id="59f40-209">fileName</span></span>|<span data-ttu-id="59f40-210">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59f40-210">String</span></span>|<span data-ttu-id="59f40-211">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="59f40-211">The name of the main Lob application file.</span></span> <span data-ttu-id="59f40-212">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="59f40-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="59f40-213">size</span><span class="sxs-lookup"><span data-stu-id="59f40-213">size</span></span>|<span data-ttu-id="59f40-214">Int64</span><span class="sxs-lookup"><span data-stu-id="59f40-214">Int64</span></span>|<span data-ttu-id="59f40-215">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="59f40-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="59f40-216">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="59f40-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="59f40-217">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="59f40-217">applicableArchitectures</span></span>|[<span data-ttu-id="59f40-218">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="59f40-218">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="59f40-219">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="59f40-219">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="59f40-220">Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="59f40-220">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="59f40-221">identityName</span><span class="sxs-lookup"><span data-stu-id="59f40-221">identityName</span></span>|<span data-ttu-id="59f40-222">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59f40-222">String</span></span>|<span data-ttu-id="59f40-223">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="59f40-223">The Identity Name.</span></span>|
|<span data-ttu-id="59f40-224">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="59f40-224">identityPublisherHash</span></span>|<span data-ttu-id="59f40-225">String</span><span class="sxs-lookup"><span data-stu-id="59f40-225">String</span></span>|<span data-ttu-id="59f40-226">O Hash do Publicador de Identidade.</span><span class="sxs-lookup"><span data-stu-id="59f40-226">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="59f40-227">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="59f40-227">identityResourceIdentifier</span></span>|<span data-ttu-id="59f40-228">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59f40-228">String</span></span>|<span data-ttu-id="59f40-229">O Identificador de Recurso da Identidade.</span><span class="sxs-lookup"><span data-stu-id="59f40-229">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="59f40-230">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="59f40-230">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="59f40-231">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="59f40-231">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="59f40-232">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="59f40-232">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="59f40-233">phoneProductIdentifier</span><span class="sxs-lookup"><span data-stu-id="59f40-233">phoneProductIdentifier</span></span>|<span data-ttu-id="59f40-234">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59f40-234">String</span></span>|<span data-ttu-id="59f40-235">O identificador do produto de telefone.</span><span class="sxs-lookup"><span data-stu-id="59f40-235">The Phone Product Identifier.</span></span>|
|<span data-ttu-id="59f40-236">phonePublisherId</span><span class="sxs-lookup"><span data-stu-id="59f40-236">phonePublisherId</span></span>|<span data-ttu-id="59f40-237">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59f40-237">String</span></span>|<span data-ttu-id="59f40-238">A ID do editor do telefone.</span><span class="sxs-lookup"><span data-stu-id="59f40-238">The Phone Publisher Id.</span></span>|
|<span data-ttu-id="59f40-239">identityVersion</span><span class="sxs-lookup"><span data-stu-id="59f40-239">identityVersion</span></span>|<span data-ttu-id="59f40-240">String</span><span class="sxs-lookup"><span data-stu-id="59f40-240">String</span></span>|<span data-ttu-id="59f40-241">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="59f40-241">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="59f40-242">Resposta</span><span class="sxs-lookup"><span data-stu-id="59f40-242">Response</span></span>
<span data-ttu-id="59f40-243">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="59f40-243">If successful, this method returns a `201 Created` response code and a [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59f40-244">Exemplo</span><span class="sxs-lookup"><span data-stu-id="59f40-244">Example</span></span>

### <a name="request"></a><span data-ttu-id="59f40-245">Solicitação</span><span class="sxs-lookup"><span data-stu-id="59f40-245">Request</span></span>
<span data-ttu-id="59f40-246">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="59f40-246">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="59f40-247">Resposta</span><span class="sxs-lookup"><span data-stu-id="59f40-247">Response</span></span>
<span data-ttu-id="59f40-p123">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="59f40-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






