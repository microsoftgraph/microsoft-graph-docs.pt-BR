---
title: Criar windowsPhone81AppX
description: Criar um novo objeto windowsPhone81AppX.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 344697be772b49994bba38b72f5d35160beb7d2e
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33934709"
---
# <a name="create-windowsphone81appx"></a><span data-ttu-id="c9176-103">Criar windowsPhone81AppX</span><span class="sxs-lookup"><span data-stu-id="c9176-103">Create windowsPhone81AppX</span></span>

> <span data-ttu-id="c9176-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c9176-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c9176-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c9176-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9176-106">Criar um novo objeto [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) .</span><span class="sxs-lookup"><span data-stu-id="c9176-106">Create a new [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c9176-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c9176-107">Prerequisites</span></span>
<span data-ttu-id="c9176-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9176-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9176-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c9176-110">Permission type</span></span>|<span data-ttu-id="c9176-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c9176-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9176-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c9176-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c9176-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9176-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c9176-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c9176-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9176-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c9176-115">Not supported.</span></span>|
|<span data-ttu-id="c9176-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c9176-116">Application</span></span>|<span data-ttu-id="c9176-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c9176-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9176-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c9176-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="c9176-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c9176-119">Request headers</span></span>
|<span data-ttu-id="c9176-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c9176-120">Header</span></span>|<span data-ttu-id="c9176-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c9176-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9176-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c9176-122">Authorization</span></span>|<span data-ttu-id="c9176-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c9176-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9176-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c9176-124">Accept</span></span>|<span data-ttu-id="c9176-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c9176-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9176-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c9176-126">Request body</span></span>
<span data-ttu-id="c9176-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsPhone81AppX.</span><span class="sxs-lookup"><span data-stu-id="c9176-127">In the request body, supply a JSON representation for the windowsPhone81AppX object.</span></span>

<span data-ttu-id="c9176-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsPhone81AppX.</span><span class="sxs-lookup"><span data-stu-id="c9176-128">The following table shows the properties that are required when you create the windowsPhone81AppX.</span></span>

|<span data-ttu-id="c9176-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c9176-129">Property</span></span>|<span data-ttu-id="c9176-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="c9176-130">Type</span></span>|<span data-ttu-id="c9176-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="c9176-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9176-132">id</span><span class="sxs-lookup"><span data-stu-id="c9176-132">id</span></span>|<span data-ttu-id="c9176-133">String</span><span class="sxs-lookup"><span data-stu-id="c9176-133">String</span></span>|<span data-ttu-id="c9176-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c9176-134">Key of the entity.</span></span> <span data-ttu-id="c9176-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c9176-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c9176-136">displayName</span><span class="sxs-lookup"><span data-stu-id="c9176-136">displayName</span></span>|<span data-ttu-id="c9176-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c9176-137">String</span></span>|<span data-ttu-id="c9176-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="c9176-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="c9176-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c9176-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c9176-140">description</span><span class="sxs-lookup"><span data-stu-id="c9176-140">description</span></span>|<span data-ttu-id="c9176-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c9176-141">String</span></span>|<span data-ttu-id="c9176-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c9176-142">The description of the app.</span></span> <span data-ttu-id="c9176-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c9176-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c9176-144">publicador</span><span class="sxs-lookup"><span data-stu-id="c9176-144">publisher</span></span>|<span data-ttu-id="c9176-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c9176-145">String</span></span>|<span data-ttu-id="c9176-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c9176-146">The publisher of the app.</span></span> <span data-ttu-id="c9176-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c9176-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c9176-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="c9176-148">largeIcon</span></span>|[<span data-ttu-id="c9176-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="c9176-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="c9176-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="c9176-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="c9176-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c9176-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c9176-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c9176-152">createdDateTime</span></span>|<span data-ttu-id="c9176-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9176-153">DateTimeOffset</span></span>|<span data-ttu-id="c9176-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c9176-154">The date and time the app was created.</span></span> <span data-ttu-id="c9176-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c9176-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c9176-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c9176-156">lastModifiedDateTime</span></span>|<span data-ttu-id="c9176-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9176-157">DateTimeOffset</span></span>|<span data-ttu-id="c9176-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="c9176-158">The date and time the app was last modified.</span></span> <span data-ttu-id="c9176-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c9176-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c9176-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="c9176-160">isFeatured</span></span>|<span data-ttu-id="c9176-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9176-161">Boolean</span></span>|<span data-ttu-id="c9176-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c9176-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c9176-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="c9176-163">privacyInformationUrl</span></span>|<span data-ttu-id="c9176-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c9176-164">String</span></span>|<span data-ttu-id="c9176-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="c9176-165">The privacy statement Url.</span></span> <span data-ttu-id="c9176-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c9176-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c9176-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="c9176-167">informationUrl</span></span>|<span data-ttu-id="c9176-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c9176-168">String</span></span>|<span data-ttu-id="c9176-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="c9176-169">The more information Url.</span></span> <span data-ttu-id="c9176-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c9176-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c9176-171">owner</span><span class="sxs-lookup"><span data-stu-id="c9176-171">owner</span></span>|<span data-ttu-id="c9176-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c9176-172">String</span></span>|<span data-ttu-id="c9176-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="c9176-173">The owner of the app.</span></span> <span data-ttu-id="c9176-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c9176-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c9176-175">developer</span><span class="sxs-lookup"><span data-stu-id="c9176-175">developer</span></span>|<span data-ttu-id="c9176-176">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c9176-176">String</span></span>|<span data-ttu-id="c9176-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c9176-177">The developer of the app.</span></span> <span data-ttu-id="c9176-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c9176-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c9176-179">notes</span><span class="sxs-lookup"><span data-stu-id="c9176-179">notes</span></span>|<span data-ttu-id="c9176-180">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c9176-180">String</span></span>|<span data-ttu-id="c9176-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c9176-181">Notes for the app.</span></span> <span data-ttu-id="c9176-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c9176-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c9176-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="c9176-183">uploadState</span></span>|<span data-ttu-id="c9176-184">Int32</span><span class="sxs-lookup"><span data-stu-id="c9176-184">Int32</span></span>|<span data-ttu-id="c9176-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="c9176-185">The upload state.</span></span> <span data-ttu-id="c9176-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c9176-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c9176-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="c9176-187">publishingState</span></span>|[<span data-ttu-id="c9176-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="c9176-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="c9176-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c9176-189">The publishing state for the app.</span></span> <span data-ttu-id="c9176-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="c9176-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="c9176-191">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c9176-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="c9176-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="c9176-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="c9176-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="c9176-193">isAssigned</span></span>|<span data-ttu-id="c9176-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9176-194">Boolean</span></span>|<span data-ttu-id="c9176-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="c9176-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="c9176-196">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c9176-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c9176-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c9176-197">roleScopeTagIds</span></span>|<span data-ttu-id="c9176-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c9176-198">String collection</span></span>|<span data-ttu-id="c9176-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="c9176-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="c9176-200">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c9176-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c9176-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="c9176-201">dependentAppCount</span></span>|<span data-ttu-id="c9176-202">Int32</span><span class="sxs-lookup"><span data-stu-id="c9176-202">Int32</span></span>|<span data-ttu-id="c9176-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="c9176-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="c9176-204">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c9176-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c9176-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="c9176-205">committedContentVersion</span></span>|<span data-ttu-id="c9176-206">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c9176-206">String</span></span>|<span data-ttu-id="c9176-207">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="c9176-207">The internal committed content version.</span></span> <span data-ttu-id="c9176-208">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="c9176-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="c9176-209">fileName</span><span class="sxs-lookup"><span data-stu-id="c9176-209">fileName</span></span>|<span data-ttu-id="c9176-210">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c9176-210">String</span></span>|<span data-ttu-id="c9176-211">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="c9176-211">The name of the main Lob application file.</span></span> <span data-ttu-id="c9176-212">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="c9176-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="c9176-213">size</span><span class="sxs-lookup"><span data-stu-id="c9176-213">size</span></span>|<span data-ttu-id="c9176-214">Int64</span><span class="sxs-lookup"><span data-stu-id="c9176-214">Int64</span></span>|<span data-ttu-id="c9176-215">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="c9176-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="c9176-216">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="c9176-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="c9176-217">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="c9176-217">applicableArchitectures</span></span>|[<span data-ttu-id="c9176-218">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="c9176-218">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="c9176-219">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="c9176-219">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="c9176-220">Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="c9176-220">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="c9176-221">identityName</span><span class="sxs-lookup"><span data-stu-id="c9176-221">identityName</span></span>|<span data-ttu-id="c9176-222">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c9176-222">String</span></span>|<span data-ttu-id="c9176-223">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="c9176-223">The Identity Name.</span></span>|
|<span data-ttu-id="c9176-224">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="c9176-224">identityPublisherHash</span></span>|<span data-ttu-id="c9176-225">String</span><span class="sxs-lookup"><span data-stu-id="c9176-225">String</span></span>|<span data-ttu-id="c9176-226">O Hash do Publicador de Identidade.</span><span class="sxs-lookup"><span data-stu-id="c9176-226">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="c9176-227">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="c9176-227">identityResourceIdentifier</span></span>|<span data-ttu-id="c9176-228">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c9176-228">String</span></span>|<span data-ttu-id="c9176-229">O Identificador de Recurso da Identidade.</span><span class="sxs-lookup"><span data-stu-id="c9176-229">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="c9176-230">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="c9176-230">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="c9176-231">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="c9176-231">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="c9176-232">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="c9176-232">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="c9176-233">phoneProductIdentifier</span><span class="sxs-lookup"><span data-stu-id="c9176-233">phoneProductIdentifier</span></span>|<span data-ttu-id="c9176-234">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c9176-234">String</span></span>|<span data-ttu-id="c9176-235">O identificador do produto de telefone.</span><span class="sxs-lookup"><span data-stu-id="c9176-235">The Phone Product Identifier.</span></span>|
|<span data-ttu-id="c9176-236">phonePublisherId</span><span class="sxs-lookup"><span data-stu-id="c9176-236">phonePublisherId</span></span>|<span data-ttu-id="c9176-237">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c9176-237">String</span></span>|<span data-ttu-id="c9176-238">A ID do editor do telefone.</span><span class="sxs-lookup"><span data-stu-id="c9176-238">The Phone Publisher Id.</span></span>|
|<span data-ttu-id="c9176-239">identityVersion</span><span class="sxs-lookup"><span data-stu-id="c9176-239">identityVersion</span></span>|<span data-ttu-id="c9176-240">String</span><span class="sxs-lookup"><span data-stu-id="c9176-240">String</span></span>|<span data-ttu-id="c9176-241">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="c9176-241">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="c9176-242">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9176-242">Response</span></span>
<span data-ttu-id="c9176-243">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c9176-243">If successful, this method returns a `201 Created` response code and a [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9176-244">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c9176-244">Example</span></span>

### <a name="request"></a><span data-ttu-id="c9176-245">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c9176-245">Request</span></span>
<span data-ttu-id="c9176-246">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c9176-246">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1467

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
    "v10_1803": true
  },
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="c9176-247">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9176-247">Response</span></span>
<span data-ttu-id="c9176-p123">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c9176-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1639

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
    "v10_1803": true
  },
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value"
}
```




