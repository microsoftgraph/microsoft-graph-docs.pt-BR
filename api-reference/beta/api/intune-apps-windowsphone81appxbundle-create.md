---
title: Criar windowsPhone81AppXBundle
description: Criar um novo objeto windowsPhone81AppXBundle.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3e0c59bcfc3a976ea0ec077444f28e854e2da465
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31798198"
---
# <a name="create-windowsphone81appxbundle"></a><span data-ttu-id="7ed6a-103">Criar windowsPhone81AppXBundle</span><span class="sxs-lookup"><span data-stu-id="7ed6a-103">Create windowsPhone81AppXBundle</span></span>

> <span data-ttu-id="7ed6a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7ed6a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7ed6a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7ed6a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ed6a-106">Criar um novo objeto [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) .</span><span class="sxs-lookup"><span data-stu-id="7ed6a-106">Create a new [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7ed6a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7ed6a-107">Prerequisites</span></span>
<span data-ttu-id="7ed6a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ed6a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ed6a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7ed6a-110">Permission type</span></span>|<span data-ttu-id="7ed6a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7ed6a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7ed6a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7ed6a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7ed6a-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ed6a-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7ed6a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7ed6a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7ed6a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7ed6a-115">Not supported.</span></span>|
|<span data-ttu-id="7ed6a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7ed6a-116">Application</span></span>|<span data-ttu-id="7ed6a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7ed6a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7ed6a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7ed6a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="7ed6a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7ed6a-119">Request headers</span></span>
|<span data-ttu-id="7ed6a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7ed6a-120">Header</span></span>|<span data-ttu-id="7ed6a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="7ed6a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7ed6a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7ed6a-122">Authorization</span></span>|<span data-ttu-id="7ed6a-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7ed6a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7ed6a-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7ed6a-124">Accept</span></span>|<span data-ttu-id="7ed6a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7ed6a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ed6a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7ed6a-126">Request body</span></span>
<span data-ttu-id="7ed6a-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsPhone81AppXBundle.</span><span class="sxs-lookup"><span data-stu-id="7ed6a-127">In the request body, supply a JSON representation for the windowsPhone81AppXBundle object.</span></span>

<span data-ttu-id="7ed6a-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsPhone81AppXBundle.</span><span class="sxs-lookup"><span data-stu-id="7ed6a-128">The following table shows the properties that are required when you create the windowsPhone81AppXBundle.</span></span>

|<span data-ttu-id="7ed6a-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7ed6a-129">Property</span></span>|<span data-ttu-id="7ed6a-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="7ed6a-130">Type</span></span>|<span data-ttu-id="7ed6a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ed6a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ed6a-132">id</span><span class="sxs-lookup"><span data-stu-id="7ed6a-132">id</span></span>|<span data-ttu-id="7ed6a-133">String</span><span class="sxs-lookup"><span data-stu-id="7ed6a-133">String</span></span>|<span data-ttu-id="7ed6a-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="7ed6a-134">Key of the entity.</span></span> <span data-ttu-id="7ed6a-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7ed6a-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ed6a-136">displayName</span><span class="sxs-lookup"><span data-stu-id="7ed6a-136">displayName</span></span>|<span data-ttu-id="7ed6a-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ed6a-137">String</span></span>|<span data-ttu-id="7ed6a-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="7ed6a-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="7ed6a-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7ed6a-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ed6a-140">description</span><span class="sxs-lookup"><span data-stu-id="7ed6a-140">description</span></span>|<span data-ttu-id="7ed6a-141">String</span><span class="sxs-lookup"><span data-stu-id="7ed6a-141">String</span></span>|<span data-ttu-id="7ed6a-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7ed6a-142">The description of the app.</span></span> <span data-ttu-id="7ed6a-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7ed6a-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ed6a-144">publicador</span><span class="sxs-lookup"><span data-stu-id="7ed6a-144">publisher</span></span>|<span data-ttu-id="7ed6a-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ed6a-145">String</span></span>|<span data-ttu-id="7ed6a-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7ed6a-146">The publisher of the app.</span></span> <span data-ttu-id="7ed6a-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7ed6a-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ed6a-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="7ed6a-148">largeIcon</span></span>|[<span data-ttu-id="7ed6a-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="7ed6a-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="7ed6a-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="7ed6a-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="7ed6a-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7ed6a-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ed6a-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7ed6a-152">createdDateTime</span></span>|<span data-ttu-id="7ed6a-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ed6a-153">DateTimeOffset</span></span>|<span data-ttu-id="7ed6a-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7ed6a-154">The date and time the app was created.</span></span> <span data-ttu-id="7ed6a-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7ed6a-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ed6a-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7ed6a-156">lastModifiedDateTime</span></span>|<span data-ttu-id="7ed6a-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ed6a-157">DateTimeOffset</span></span>|<span data-ttu-id="7ed6a-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="7ed6a-158">The date and time the app was last modified.</span></span> <span data-ttu-id="7ed6a-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7ed6a-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ed6a-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="7ed6a-160">isFeatured</span></span>|<span data-ttu-id="7ed6a-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ed6a-161">Boolean</span></span>|<span data-ttu-id="7ed6a-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7ed6a-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ed6a-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="7ed6a-163">privacyInformationUrl</span></span>|<span data-ttu-id="7ed6a-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ed6a-164">String</span></span>|<span data-ttu-id="7ed6a-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="7ed6a-165">The privacy statement Url.</span></span> <span data-ttu-id="7ed6a-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7ed6a-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ed6a-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="7ed6a-167">informationUrl</span></span>|<span data-ttu-id="7ed6a-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ed6a-168">String</span></span>|<span data-ttu-id="7ed6a-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="7ed6a-169">The more information Url.</span></span> <span data-ttu-id="7ed6a-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7ed6a-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ed6a-171">owner</span><span class="sxs-lookup"><span data-stu-id="7ed6a-171">owner</span></span>|<span data-ttu-id="7ed6a-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ed6a-172">String</span></span>|<span data-ttu-id="7ed6a-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="7ed6a-173">The owner of the app.</span></span> <span data-ttu-id="7ed6a-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7ed6a-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ed6a-175">developer</span><span class="sxs-lookup"><span data-stu-id="7ed6a-175">developer</span></span>|<span data-ttu-id="7ed6a-176">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ed6a-176">String</span></span>|<span data-ttu-id="7ed6a-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7ed6a-177">The developer of the app.</span></span> <span data-ttu-id="7ed6a-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7ed6a-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ed6a-179">notes</span><span class="sxs-lookup"><span data-stu-id="7ed6a-179">notes</span></span>|<span data-ttu-id="7ed6a-180">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ed6a-180">String</span></span>|<span data-ttu-id="7ed6a-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7ed6a-181">Notes for the app.</span></span> <span data-ttu-id="7ed6a-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7ed6a-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ed6a-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="7ed6a-183">uploadState</span></span>|<span data-ttu-id="7ed6a-184">Int32</span><span class="sxs-lookup"><span data-stu-id="7ed6a-184">Int32</span></span>|<span data-ttu-id="7ed6a-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="7ed6a-185">The upload state.</span></span> <span data-ttu-id="7ed6a-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7ed6a-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ed6a-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="7ed6a-187">publishingState</span></span>|[<span data-ttu-id="7ed6a-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="7ed6a-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="7ed6a-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7ed6a-189">The publishing state for the app.</span></span> <span data-ttu-id="7ed6a-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="7ed6a-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="7ed6a-191">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7ed6a-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="7ed6a-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="7ed6a-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="7ed6a-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="7ed6a-193">isAssigned</span></span>|<span data-ttu-id="7ed6a-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ed6a-194">Boolean</span></span>|<span data-ttu-id="7ed6a-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="7ed6a-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="7ed6a-196">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7ed6a-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ed6a-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7ed6a-197">roleScopeTagIds</span></span>|<span data-ttu-id="7ed6a-198">Coleção String</span><span class="sxs-lookup"><span data-stu-id="7ed6a-198">String collection</span></span>|<span data-ttu-id="7ed6a-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="7ed6a-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="7ed6a-200">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7ed6a-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ed6a-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="7ed6a-201">dependentAppCount</span></span>|<span data-ttu-id="7ed6a-202">Int32</span><span class="sxs-lookup"><span data-stu-id="7ed6a-202">Int32</span></span>|<span data-ttu-id="7ed6a-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="7ed6a-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="7ed6a-204">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7ed6a-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ed6a-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="7ed6a-205">committedContentVersion</span></span>|<span data-ttu-id="7ed6a-206">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ed6a-206">String</span></span>|<span data-ttu-id="7ed6a-207">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="7ed6a-207">The internal committed content version.</span></span> <span data-ttu-id="7ed6a-208">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="7ed6a-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="7ed6a-209">fileName</span><span class="sxs-lookup"><span data-stu-id="7ed6a-209">fileName</span></span>|<span data-ttu-id="7ed6a-210">String</span><span class="sxs-lookup"><span data-stu-id="7ed6a-210">String</span></span>|<span data-ttu-id="7ed6a-211">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="7ed6a-211">The name of the main Lob application file.</span></span> <span data-ttu-id="7ed6a-212">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="7ed6a-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="7ed6a-213">size</span><span class="sxs-lookup"><span data-stu-id="7ed6a-213">size</span></span>|<span data-ttu-id="7ed6a-214">Int64</span><span class="sxs-lookup"><span data-stu-id="7ed6a-214">Int64</span></span>|<span data-ttu-id="7ed6a-215">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="7ed6a-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="7ed6a-216">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="7ed6a-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="7ed6a-217">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="7ed6a-217">applicableArchitectures</span></span>|[<span data-ttu-id="7ed6a-218">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="7ed6a-218">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="7ed6a-219">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="7ed6a-219">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="7ed6a-220">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span><span class="sxs-lookup"><span data-stu-id="7ed6a-220">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span></span> <span data-ttu-id="7ed6a-221">Os valores possíveis são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="7ed6a-221">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="7ed6a-222">identityName</span><span class="sxs-lookup"><span data-stu-id="7ed6a-222">identityName</span></span>|<span data-ttu-id="7ed6a-223">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ed6a-223">String</span></span>|<span data-ttu-id="7ed6a-224">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="7ed6a-224">The Identity Name.</span></span> <span data-ttu-id="7ed6a-225">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="7ed6a-225">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="7ed6a-226">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="7ed6a-226">identityPublisherHash</span></span>|<span data-ttu-id="7ed6a-227">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ed6a-227">String</span></span>|<span data-ttu-id="7ed6a-228">O Hash do Publicador de Identidade.</span><span class="sxs-lookup"><span data-stu-id="7ed6a-228">The Identity Publisher Hash.</span></span> <span data-ttu-id="7ed6a-229">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="7ed6a-229">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="7ed6a-230">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="7ed6a-230">identityResourceIdentifier</span></span>|<span data-ttu-id="7ed6a-231">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ed6a-231">String</span></span>|<span data-ttu-id="7ed6a-232">O Identificador de Recurso da Identidade.</span><span class="sxs-lookup"><span data-stu-id="7ed6a-232">The Identity Resource Identifier.</span></span> <span data-ttu-id="7ed6a-233">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="7ed6a-233">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="7ed6a-234">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="7ed6a-234">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="7ed6a-235">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="7ed6a-235">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="7ed6a-236">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="7ed6a-236">The value for the minimum applicable operating system.</span></span> <span data-ttu-id="7ed6a-237">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="7ed6a-237">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="7ed6a-238">phoneProductIdentifier</span><span class="sxs-lookup"><span data-stu-id="7ed6a-238">phoneProductIdentifier</span></span>|<span data-ttu-id="7ed6a-239">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ed6a-239">String</span></span>|<span data-ttu-id="7ed6a-240">O identificador do produto de telefone.</span><span class="sxs-lookup"><span data-stu-id="7ed6a-240">The Phone Product Identifier.</span></span> <span data-ttu-id="7ed6a-241">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="7ed6a-241">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="7ed6a-242">phonePublisherId</span><span class="sxs-lookup"><span data-stu-id="7ed6a-242">phonePublisherId</span></span>|<span data-ttu-id="7ed6a-243">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ed6a-243">String</span></span>|<span data-ttu-id="7ed6a-244">A ID do editor do telefone. herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="7ed6a-244">The Phone Publisher Id. Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="7ed6a-245">identityVersion</span><span class="sxs-lookup"><span data-stu-id="7ed6a-245">identityVersion</span></span>|<span data-ttu-id="7ed6a-246">String</span><span class="sxs-lookup"><span data-stu-id="7ed6a-246">String</span></span>|<span data-ttu-id="7ed6a-247">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="7ed6a-247">The identity version.</span></span> <span data-ttu-id="7ed6a-248">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="7ed6a-248">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="7ed6a-249">appXPackageInformationList</span><span class="sxs-lookup"><span data-stu-id="7ed6a-249">appXPackageInformationList</span></span>|<span data-ttu-id="7ed6a-250">coleção [windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md)</span><span class="sxs-lookup"><span data-stu-id="7ed6a-250">[windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md) collection</span></span>|<span data-ttu-id="7ed6a-251">A lista de informações do pacote AppX.</span><span class="sxs-lookup"><span data-stu-id="7ed6a-251">The list of AppX Package Information.</span></span>|



## <a name="response"></a><span data-ttu-id="7ed6a-252">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ed6a-252">Response</span></span>
<span data-ttu-id="7ed6a-253">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7ed6a-253">If successful, this method returns a `201 Created` response code and a [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ed6a-254">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7ed6a-254">Example</span></span>

### <a name="request"></a><span data-ttu-id="7ed6a-255">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7ed6a-255">Request</span></span>
<span data-ttu-id="7ed6a-256">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7ed6a-256">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 2211

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
    "v10_1803": true
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
        "v10_1803": true
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="7ed6a-257">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ed6a-257">Response</span></span>
<span data-ttu-id="7ed6a-p129">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7ed6a-p129">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2383

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
    "v10_1803": true
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
        "v10_1803": true
      }
    }
  ]
}
```





