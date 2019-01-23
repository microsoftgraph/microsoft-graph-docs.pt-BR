---
title: Criar androidLobApp
description: Cria um novo objeto androidLobApp.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4d08ae1af5c5415c22c70d45e3d7a0c264e3069f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399231"
---
# <a name="create-androidlobapp"></a><span data-ttu-id="18a79-103">Criar androidLobApp</span><span class="sxs-lookup"><span data-stu-id="18a79-103">Create androidLobApp</span></span>

> <span data-ttu-id="18a79-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="18a79-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="18a79-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="18a79-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="18a79-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="18a79-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18a79-107">Cria um novo objeto [androidLobApp](../resources/intune-apps-androidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="18a79-107">Create a new [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="18a79-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="18a79-108">Prerequisites</span></span>
<span data-ttu-id="18a79-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="18a79-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="18a79-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="18a79-111">Permission type</span></span>|<span data-ttu-id="18a79-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="18a79-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18a79-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="18a79-113">Delegated (work or school account)</span></span>|<span data-ttu-id="18a79-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18a79-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="18a79-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="18a79-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18a79-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="18a79-116">Not supported.</span></span>|
|<span data-ttu-id="18a79-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="18a79-117">Application</span></span>|<span data-ttu-id="18a79-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="18a79-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="18a79-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="18a79-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="18a79-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="18a79-120">Request headers</span></span>
|<span data-ttu-id="18a79-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="18a79-121">Header</span></span>|<span data-ttu-id="18a79-122">Valor</span><span class="sxs-lookup"><span data-stu-id="18a79-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18a79-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="18a79-123">Authorization</span></span>|<span data-ttu-id="18a79-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="18a79-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18a79-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="18a79-125">Accept</span></span>|<span data-ttu-id="18a79-126">application/json</span><span class="sxs-lookup"><span data-stu-id="18a79-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18a79-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="18a79-127">Request body</span></span>
<span data-ttu-id="18a79-128">No corpo da solicitação, forneça uma representação JSON do objeto androidLobApp.</span><span class="sxs-lookup"><span data-stu-id="18a79-128">In the request body, supply a JSON representation for the androidLobApp object.</span></span>

<span data-ttu-id="18a79-129">A tabela a seguir mostra as propriedades obrigatórias ao criar androidLobApp.</span><span class="sxs-lookup"><span data-stu-id="18a79-129">The following table shows the properties that are required when you create the androidLobApp.</span></span>

|<span data-ttu-id="18a79-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="18a79-130">Property</span></span>|<span data-ttu-id="18a79-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="18a79-131">Type</span></span>|<span data-ttu-id="18a79-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="18a79-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18a79-133">id</span><span class="sxs-lookup"><span data-stu-id="18a79-133">id</span></span>|<span data-ttu-id="18a79-134">String</span><span class="sxs-lookup"><span data-stu-id="18a79-134">String</span></span>|<span data-ttu-id="18a79-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="18a79-135">Key of the entity.</span></span> <span data-ttu-id="18a79-136">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18a79-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18a79-137">displayName</span><span class="sxs-lookup"><span data-stu-id="18a79-137">displayName</span></span>|<span data-ttu-id="18a79-138">String</span><span class="sxs-lookup"><span data-stu-id="18a79-138">String</span></span>|<span data-ttu-id="18a79-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="18a79-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="18a79-140">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18a79-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18a79-141">description</span><span class="sxs-lookup"><span data-stu-id="18a79-141">description</span></span>|<span data-ttu-id="18a79-142">String</span><span class="sxs-lookup"><span data-stu-id="18a79-142">String</span></span>|<span data-ttu-id="18a79-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="18a79-143">The description of the app.</span></span> <span data-ttu-id="18a79-144">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18a79-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18a79-145">publisher</span><span class="sxs-lookup"><span data-stu-id="18a79-145">publisher</span></span>|<span data-ttu-id="18a79-146">String</span><span class="sxs-lookup"><span data-stu-id="18a79-146">String</span></span>|<span data-ttu-id="18a79-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="18a79-147">The publisher of the app.</span></span> <span data-ttu-id="18a79-148">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18a79-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18a79-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="18a79-149">largeIcon</span></span>|[<span data-ttu-id="18a79-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="18a79-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="18a79-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="18a79-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="18a79-152">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18a79-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18a79-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="18a79-153">createdDateTime</span></span>|<span data-ttu-id="18a79-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18a79-154">DateTimeOffset</span></span>|<span data-ttu-id="18a79-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="18a79-155">The date and time the app was created.</span></span> <span data-ttu-id="18a79-156">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18a79-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18a79-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="18a79-157">lastModifiedDateTime</span></span>|<span data-ttu-id="18a79-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18a79-158">DateTimeOffset</span></span>|<span data-ttu-id="18a79-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="18a79-159">The date and time the app was last modified.</span></span> <span data-ttu-id="18a79-160">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18a79-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18a79-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="18a79-161">isFeatured</span></span>|<span data-ttu-id="18a79-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="18a79-162">Boolean</span></span>|<span data-ttu-id="18a79-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18a79-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18a79-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="18a79-164">privacyInformationUrl</span></span>|<span data-ttu-id="18a79-165">String</span><span class="sxs-lookup"><span data-stu-id="18a79-165">String</span></span>|<span data-ttu-id="18a79-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="18a79-166">The privacy statement Url.</span></span> <span data-ttu-id="18a79-167">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18a79-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18a79-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="18a79-168">informationUrl</span></span>|<span data-ttu-id="18a79-169">String</span><span class="sxs-lookup"><span data-stu-id="18a79-169">String</span></span>|<span data-ttu-id="18a79-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="18a79-170">The more information Url.</span></span> <span data-ttu-id="18a79-171">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18a79-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18a79-172">owner</span><span class="sxs-lookup"><span data-stu-id="18a79-172">owner</span></span>|<span data-ttu-id="18a79-173">String</span><span class="sxs-lookup"><span data-stu-id="18a79-173">String</span></span>|<span data-ttu-id="18a79-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="18a79-174">The owner of the app.</span></span> <span data-ttu-id="18a79-175">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18a79-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18a79-176">developer</span><span class="sxs-lookup"><span data-stu-id="18a79-176">developer</span></span>|<span data-ttu-id="18a79-177">String</span><span class="sxs-lookup"><span data-stu-id="18a79-177">String</span></span>|<span data-ttu-id="18a79-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="18a79-178">The developer of the app.</span></span> <span data-ttu-id="18a79-179">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18a79-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18a79-180">Observações</span><span class="sxs-lookup"><span data-stu-id="18a79-180">notes</span></span>|<span data-ttu-id="18a79-181">String</span><span class="sxs-lookup"><span data-stu-id="18a79-181">String</span></span>|<span data-ttu-id="18a79-182">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="18a79-182">Notes for the app.</span></span> <span data-ttu-id="18a79-183">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18a79-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18a79-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="18a79-184">uploadState</span></span>|<span data-ttu-id="18a79-185">Int32</span><span class="sxs-lookup"><span data-stu-id="18a79-185">Int32</span></span>|<span data-ttu-id="18a79-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="18a79-186">The upload state.</span></span> <span data-ttu-id="18a79-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18a79-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18a79-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="18a79-188">publishingState</span></span>|[<span data-ttu-id="18a79-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="18a79-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="18a79-190">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="18a79-190">The publishing state for the app.</span></span> <span data-ttu-id="18a79-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="18a79-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="18a79-192">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="18a79-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="18a79-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="18a79-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="18a79-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="18a79-194">isAssigned</span></span>|<span data-ttu-id="18a79-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="18a79-195">Boolean</span></span>|<span data-ttu-id="18a79-196">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="18a79-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="18a79-197">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18a79-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18a79-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="18a79-198">roleScopeTagIds</span></span>|<span data-ttu-id="18a79-199">String collection</span><span class="sxs-lookup"><span data-stu-id="18a79-199">String collection</span></span>|<span data-ttu-id="18a79-200">Lista de ids de marca de escopo para esse aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="18a79-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="18a79-201">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18a79-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18a79-202">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="18a79-202">committedContentVersion</span></span>|<span data-ttu-id="18a79-203">String</span><span class="sxs-lookup"><span data-stu-id="18a79-203">String</span></span>|<span data-ttu-id="18a79-204">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="18a79-204">The internal committed content version.</span></span> <span data-ttu-id="18a79-205">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="18a79-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="18a79-206">fileName</span><span class="sxs-lookup"><span data-stu-id="18a79-206">fileName</span></span>|<span data-ttu-id="18a79-207">String</span><span class="sxs-lookup"><span data-stu-id="18a79-207">String</span></span>|<span data-ttu-id="18a79-208">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="18a79-208">The name of the main Lob application file.</span></span> <span data-ttu-id="18a79-209">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="18a79-209">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="18a79-210">size</span><span class="sxs-lookup"><span data-stu-id="18a79-210">size</span></span>|<span data-ttu-id="18a79-211">Int64</span><span class="sxs-lookup"><span data-stu-id="18a79-211">Int64</span></span>|<span data-ttu-id="18a79-212">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="18a79-212">The total size, including all uploaded files.</span></span> <span data-ttu-id="18a79-213">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="18a79-213">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="18a79-214">packageId</span><span class="sxs-lookup"><span data-stu-id="18a79-214">packageId</span></span>|<span data-ttu-id="18a79-215">String</span><span class="sxs-lookup"><span data-stu-id="18a79-215">String</span></span>|<span data-ttu-id="18a79-216">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="18a79-216">The package identifier.</span></span>|
|<span data-ttu-id="18a79-217">identityName</span><span class="sxs-lookup"><span data-stu-id="18a79-217">identityName</span></span>|<span data-ttu-id="18a79-218">String</span><span class="sxs-lookup"><span data-stu-id="18a79-218">String</span></span>|<span data-ttu-id="18a79-219">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="18a79-219">The Identity Name.</span></span>|
|<span data-ttu-id="18a79-220">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="18a79-220">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="18a79-221">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="18a79-221">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="18a79-222">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="18a79-222">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="18a79-223">versionName</span><span class="sxs-lookup"><span data-stu-id="18a79-223">versionName</span></span>|<span data-ttu-id="18a79-224">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18a79-224">String</span></span>|<span data-ttu-id="18a79-225">O nome da versão do aplicativo de Linha de Negócios (LoB) Android.</span><span class="sxs-lookup"><span data-stu-id="18a79-225">The version name of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="18a79-226">versionCode</span><span class="sxs-lookup"><span data-stu-id="18a79-226">versionCode</span></span>|<span data-ttu-id="18a79-227">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18a79-227">String</span></span>|<span data-ttu-id="18a79-228">O código da versão do aplicativo de Linha de Negócios (LoB) Android.</span><span class="sxs-lookup"><span data-stu-id="18a79-228">The version code of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="18a79-229">identityVersion</span><span class="sxs-lookup"><span data-stu-id="18a79-229">identityVersion</span></span>|<span data-ttu-id="18a79-230">String</span><span class="sxs-lookup"><span data-stu-id="18a79-230">String</span></span>|<span data-ttu-id="18a79-231">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="18a79-231">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="18a79-232">Resposta</span><span class="sxs-lookup"><span data-stu-id="18a79-232">Response</span></span>
<span data-ttu-id="18a79-233">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [androidLobApp](../resources/intune-apps-androidlobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="18a79-233">If successful, this method returns a `201 Created` response code and a [androidLobApp](../resources/intune-apps-androidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18a79-234">Exemplo</span><span class="sxs-lookup"><span data-stu-id="18a79-234">Example</span></span>

### <a name="request"></a><span data-ttu-id="18a79-235">Solicitação</span><span class="sxs-lookup"><span data-stu-id="18a79-235">Request</span></span>
<span data-ttu-id="18a79-236">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="18a79-236">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1386

{
  "@odata.type": "#microsoft.graph.androidLobApp",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
  "identityName": "Identity Name value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="18a79-237">Resposta</span><span class="sxs-lookup"><span data-stu-id="18a79-237">Response</span></span>
<span data-ttu-id="18a79-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="18a79-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1558

{
  "@odata.type": "#microsoft.graph.androidLobApp",
  "id": "4b9a27d0-27d0-4b9a-d027-9a4bd0279a4b",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
  "identityName": "Identity Name value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```




