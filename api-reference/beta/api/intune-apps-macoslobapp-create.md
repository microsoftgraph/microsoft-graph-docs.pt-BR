---
title: Criar macOSLobApp
description: Crie um novo objeto de macOSLobApp.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 264bc1e104e7b582f3a15f38d2f5a8a585095789
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418096"
---
# <a name="create-macoslobapp"></a><span data-ttu-id="55afa-103">Criar macOSLobApp</span><span class="sxs-lookup"><span data-stu-id="55afa-103">Create macOSLobApp</span></span>

> <span data-ttu-id="55afa-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="55afa-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="55afa-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="55afa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="55afa-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="55afa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55afa-107">Crie um novo objeto de [macOSLobApp](../resources/intune-apps-macoslobapp.md) .</span><span class="sxs-lookup"><span data-stu-id="55afa-107">Create a new [macOSLobApp](../resources/intune-apps-macoslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="55afa-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="55afa-108">Prerequisites</span></span>
<span data-ttu-id="55afa-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="55afa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="55afa-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="55afa-111">Permission type</span></span>|<span data-ttu-id="55afa-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="55afa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="55afa-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="55afa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="55afa-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55afa-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="55afa-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="55afa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="55afa-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="55afa-116">Not supported.</span></span>|
|<span data-ttu-id="55afa-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="55afa-117">Application</span></span>|<span data-ttu-id="55afa-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="55afa-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="55afa-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="55afa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="55afa-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="55afa-120">Request headers</span></span>
|<span data-ttu-id="55afa-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="55afa-121">Header</span></span>|<span data-ttu-id="55afa-122">Valor</span><span class="sxs-lookup"><span data-stu-id="55afa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="55afa-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="55afa-123">Authorization</span></span>|<span data-ttu-id="55afa-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="55afa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="55afa-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="55afa-125">Accept</span></span>|<span data-ttu-id="55afa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="55afa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="55afa-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="55afa-127">Request body</span></span>
<span data-ttu-id="55afa-128">No corpo da solicitação, fornece uma representação JSON para o objeto macOSLobApp.</span><span class="sxs-lookup"><span data-stu-id="55afa-128">In the request body, supply a JSON representation for the macOSLobApp object.</span></span>

<span data-ttu-id="55afa-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o macOSLobApp.</span><span class="sxs-lookup"><span data-stu-id="55afa-129">The following table shows the properties that are required when you create the macOSLobApp.</span></span>

|<span data-ttu-id="55afa-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="55afa-130">Property</span></span>|<span data-ttu-id="55afa-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="55afa-131">Type</span></span>|<span data-ttu-id="55afa-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="55afa-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55afa-133">id</span><span class="sxs-lookup"><span data-stu-id="55afa-133">id</span></span>|<span data-ttu-id="55afa-134">String</span><span class="sxs-lookup"><span data-stu-id="55afa-134">String</span></span>|<span data-ttu-id="55afa-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="55afa-135">Key of the entity.</span></span> <span data-ttu-id="55afa-136">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="55afa-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="55afa-137">displayName</span><span class="sxs-lookup"><span data-stu-id="55afa-137">displayName</span></span>|<span data-ttu-id="55afa-138">String</span><span class="sxs-lookup"><span data-stu-id="55afa-138">String</span></span>|<span data-ttu-id="55afa-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="55afa-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="55afa-140">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="55afa-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="55afa-141">description</span><span class="sxs-lookup"><span data-stu-id="55afa-141">description</span></span>|<span data-ttu-id="55afa-142">String</span><span class="sxs-lookup"><span data-stu-id="55afa-142">String</span></span>|<span data-ttu-id="55afa-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="55afa-143">The description of the app.</span></span> <span data-ttu-id="55afa-144">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="55afa-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="55afa-145">publisher</span><span class="sxs-lookup"><span data-stu-id="55afa-145">publisher</span></span>|<span data-ttu-id="55afa-146">String</span><span class="sxs-lookup"><span data-stu-id="55afa-146">String</span></span>|<span data-ttu-id="55afa-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="55afa-147">The publisher of the app.</span></span> <span data-ttu-id="55afa-148">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="55afa-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="55afa-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="55afa-149">largeIcon</span></span>|[<span data-ttu-id="55afa-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="55afa-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="55afa-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="55afa-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="55afa-152">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="55afa-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="55afa-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="55afa-153">createdDateTime</span></span>|<span data-ttu-id="55afa-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55afa-154">DateTimeOffset</span></span>|<span data-ttu-id="55afa-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="55afa-155">The date and time the app was created.</span></span> <span data-ttu-id="55afa-156">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="55afa-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="55afa-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="55afa-157">lastModifiedDateTime</span></span>|<span data-ttu-id="55afa-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55afa-158">DateTimeOffset</span></span>|<span data-ttu-id="55afa-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="55afa-159">The date and time the app was last modified.</span></span> <span data-ttu-id="55afa-160">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="55afa-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="55afa-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="55afa-161">isFeatured</span></span>|<span data-ttu-id="55afa-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="55afa-162">Boolean</span></span>|<span data-ttu-id="55afa-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="55afa-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="55afa-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="55afa-164">privacyInformationUrl</span></span>|<span data-ttu-id="55afa-165">String</span><span class="sxs-lookup"><span data-stu-id="55afa-165">String</span></span>|<span data-ttu-id="55afa-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="55afa-166">The privacy statement Url.</span></span> <span data-ttu-id="55afa-167">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="55afa-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="55afa-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="55afa-168">informationUrl</span></span>|<span data-ttu-id="55afa-169">String</span><span class="sxs-lookup"><span data-stu-id="55afa-169">String</span></span>|<span data-ttu-id="55afa-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="55afa-170">The more information Url.</span></span> <span data-ttu-id="55afa-171">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="55afa-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="55afa-172">owner</span><span class="sxs-lookup"><span data-stu-id="55afa-172">owner</span></span>|<span data-ttu-id="55afa-173">String</span><span class="sxs-lookup"><span data-stu-id="55afa-173">String</span></span>|<span data-ttu-id="55afa-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="55afa-174">The owner of the app.</span></span> <span data-ttu-id="55afa-175">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="55afa-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="55afa-176">developer</span><span class="sxs-lookup"><span data-stu-id="55afa-176">developer</span></span>|<span data-ttu-id="55afa-177">String</span><span class="sxs-lookup"><span data-stu-id="55afa-177">String</span></span>|<span data-ttu-id="55afa-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="55afa-178">The developer of the app.</span></span> <span data-ttu-id="55afa-179">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="55afa-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="55afa-180">Observações</span><span class="sxs-lookup"><span data-stu-id="55afa-180">notes</span></span>|<span data-ttu-id="55afa-181">String</span><span class="sxs-lookup"><span data-stu-id="55afa-181">String</span></span>|<span data-ttu-id="55afa-182">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="55afa-182">Notes for the app.</span></span> <span data-ttu-id="55afa-183">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="55afa-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="55afa-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="55afa-184">uploadState</span></span>|<span data-ttu-id="55afa-185">Int32</span><span class="sxs-lookup"><span data-stu-id="55afa-185">Int32</span></span>|<span data-ttu-id="55afa-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="55afa-186">The upload state.</span></span> <span data-ttu-id="55afa-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="55afa-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="55afa-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="55afa-188">publishingState</span></span>|[<span data-ttu-id="55afa-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="55afa-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="55afa-190">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="55afa-190">The publishing state for the app.</span></span> <span data-ttu-id="55afa-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="55afa-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="55afa-192">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="55afa-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="55afa-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="55afa-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="55afa-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="55afa-194">isAssigned</span></span>|<span data-ttu-id="55afa-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="55afa-195">Boolean</span></span>|<span data-ttu-id="55afa-196">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="55afa-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="55afa-197">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="55afa-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="55afa-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="55afa-198">roleScopeTagIds</span></span>|<span data-ttu-id="55afa-199">String collection</span><span class="sxs-lookup"><span data-stu-id="55afa-199">String collection</span></span>|<span data-ttu-id="55afa-200">Lista de ids de marca de escopo para esse aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="55afa-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="55afa-201">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="55afa-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="55afa-202">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="55afa-202">committedContentVersion</span></span>|<span data-ttu-id="55afa-203">String</span><span class="sxs-lookup"><span data-stu-id="55afa-203">String</span></span>|<span data-ttu-id="55afa-204">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="55afa-204">The internal committed content version.</span></span> <span data-ttu-id="55afa-205">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="55afa-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="55afa-206">fileName</span><span class="sxs-lookup"><span data-stu-id="55afa-206">fileName</span></span>|<span data-ttu-id="55afa-207">String</span><span class="sxs-lookup"><span data-stu-id="55afa-207">String</span></span>|<span data-ttu-id="55afa-208">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="55afa-208">The name of the main Lob application file.</span></span> <span data-ttu-id="55afa-209">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="55afa-209">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="55afa-210">size</span><span class="sxs-lookup"><span data-stu-id="55afa-210">size</span></span>|<span data-ttu-id="55afa-211">Int64</span><span class="sxs-lookup"><span data-stu-id="55afa-211">Int64</span></span>|<span data-ttu-id="55afa-212">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="55afa-212">The total size, including all uploaded files.</span></span> <span data-ttu-id="55afa-213">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="55afa-213">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="55afa-214">bundleId</span><span class="sxs-lookup"><span data-stu-id="55afa-214">bundleId</span></span>|<span data-ttu-id="55afa-215">String</span><span class="sxs-lookup"><span data-stu-id="55afa-215">String</span></span>|<span data-ttu-id="55afa-216">A id do pacote.</span><span class="sxs-lookup"><span data-stu-id="55afa-216">The bundle id.</span></span>|
|<span data-ttu-id="55afa-217">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="55afa-217">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="55afa-218">macOSMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="55afa-218">macOSMinimumOperatingSystem</span></span>](../resources/intune-apps-macosminimumoperatingsystem.md)|<span data-ttu-id="55afa-219">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="55afa-219">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="55afa-220">buildNumber</span><span class="sxs-lookup"><span data-stu-id="55afa-220">buildNumber</span></span>|<span data-ttu-id="55afa-221">String</span><span class="sxs-lookup"><span data-stu-id="55afa-221">String</span></span>|<span data-ttu-id="55afa-222">O número de compilação da linha de MacOS do aplicativo de negócios (LoB).</span><span class="sxs-lookup"><span data-stu-id="55afa-222">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="55afa-223">versionNumber</span><span class="sxs-lookup"><span data-stu-id="55afa-223">versionNumber</span></span>|<span data-ttu-id="55afa-224">String</span><span class="sxs-lookup"><span data-stu-id="55afa-224">String</span></span>|<span data-ttu-id="55afa-225">O número de versão da linha de MacOS do aplicativo de negócios (LoB).</span><span class="sxs-lookup"><span data-stu-id="55afa-225">The version number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="55afa-226">childApps</span><span class="sxs-lookup"><span data-stu-id="55afa-226">childApps</span></span>|<span data-ttu-id="55afa-227">coleção [macOSLobChildApp](../resources/intune-apps-macoslobchildapp.md)</span><span class="sxs-lookup"><span data-stu-id="55afa-227">[macOSLobChildApp](../resources/intune-apps-macoslobchildapp.md) collection</span></span>|<span data-ttu-id="55afa-228">A lista neste pacote do pacote de aplicativo</span><span class="sxs-lookup"><span data-stu-id="55afa-228">The app list in this bundle package</span></span>|
|<span data-ttu-id="55afa-229">identityVersion</span><span class="sxs-lookup"><span data-stu-id="55afa-229">identityVersion</span></span>|<span data-ttu-id="55afa-230">String</span><span class="sxs-lookup"><span data-stu-id="55afa-230">String</span></span>|<span data-ttu-id="55afa-231">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="55afa-231">The identity version.</span></span>|
|<span data-ttu-id="55afa-232">md5HashChunkSize</span><span class="sxs-lookup"><span data-stu-id="55afa-232">md5HashChunkSize</span></span>|<span data-ttu-id="55afa-233">Int32</span><span class="sxs-lookup"><span data-stu-id="55afa-233">Int32</span></span>|<span data-ttu-id="55afa-234">O tamanho do bloco de hash MD5</span><span class="sxs-lookup"><span data-stu-id="55afa-234">The chunk size for MD5 hash</span></span>|
|<span data-ttu-id="55afa-235">md5Hash</span><span class="sxs-lookup"><span data-stu-id="55afa-235">md5Hash</span></span>|<span data-ttu-id="55afa-236">String collection</span><span class="sxs-lookup"><span data-stu-id="55afa-236">String collection</span></span>|<span data-ttu-id="55afa-237">Os códigos de hash MD5</span><span class="sxs-lookup"><span data-stu-id="55afa-237">The MD5 hash codes</span></span>|
|<span data-ttu-id="55afa-238">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="55afa-238">ignoreVersionDetection</span></span>|<span data-ttu-id="55afa-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="55afa-239">Boolean</span></span>|<span data-ttu-id="55afa-240">Um booliano para controlar se a versão do aplicativo será usada para detectar o aplicativo depois que ele for instalado em um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="55afa-240">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="55afa-241">Defina essa opção para verdadeiro para macOS aplicativos de linha de negócios (LoB) que usam um recurso de atualização self.</span><span class="sxs-lookup"><span data-stu-id="55afa-241">Set this to true for macOS Line of Business (LoB) apps that use a self update feature.</span></span>|



## <a name="response"></a><span data-ttu-id="55afa-242">Resposta</span><span class="sxs-lookup"><span data-stu-id="55afa-242">Response</span></span>
<span data-ttu-id="55afa-243">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [macOSLobApp](../resources/intune-apps-macoslobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="55afa-243">If successful, this method returns a `201 Created` response code and a [macOSLobApp](../resources/intune-apps-macoslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55afa-244">Exemplo</span><span class="sxs-lookup"><span data-stu-id="55afa-244">Example</span></span>

### <a name="request"></a><span data-ttu-id="55afa-245">Solicitação</span><span class="sxs-lookup"><span data-stu-id="55afa-245">Request</span></span>
<span data-ttu-id="55afa-246">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="55afa-246">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1547

{
  "@odata.type": "#microsoft.graph.macOSLobApp",
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
  "bundleId": "Bundle Id value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.macOSMinimumOperatingSystem",
    "v10_7": true,
    "v10_8": true,
    "v10_9": true,
    "v10_10": true,
    "v10_11": true,
    "v10_12": true,
    "v10_13": true
  },
  "buildNumber": "Build Number value",
  "versionNumber": "Version Number value",
  "childApps": [
    {
      "@odata.type": "microsoft.graph.macOSLobChildApp",
      "bundleId": "Bundle Id value",
      "buildNumber": "Build Number value",
      "versionNumber": "Version Number value"
    }
  ],
  "identityVersion": "Identity Version value",
  "md5HashChunkSize": 0,
  "md5Hash": [
    "Md5Hash value"
  ],
  "ignoreVersionDetection": true
}
```

### <a name="response"></a><span data-ttu-id="55afa-247">Resposta</span><span class="sxs-lookup"><span data-stu-id="55afa-247">Response</span></span>
<span data-ttu-id="55afa-p123">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="55afa-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1719

{
  "@odata.type": "#microsoft.graph.macOSLobApp",
  "id": "7be9250a-250a-7be9-0a25-e97b0a25e97b",
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
  "bundleId": "Bundle Id value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.macOSMinimumOperatingSystem",
    "v10_7": true,
    "v10_8": true,
    "v10_9": true,
    "v10_10": true,
    "v10_11": true,
    "v10_12": true,
    "v10_13": true
  },
  "buildNumber": "Build Number value",
  "versionNumber": "Version Number value",
  "childApps": [
    {
      "@odata.type": "microsoft.graph.macOSLobChildApp",
      "bundleId": "Bundle Id value",
      "buildNumber": "Build Number value",
      "versionNumber": "Version Number value"
    }
  ],
  "identityVersion": "Identity Version value",
  "md5HashChunkSize": 0,
  "md5Hash": [
    "Md5Hash value"
  ],
  "ignoreVersionDetection": true
}
```




