---
title: Visão geral dos registros de chamadas
description: Os registros de chamadas fornecem informações sobre as chamadas e reuniões que ocorrem em sua organização.
author: stephenjust
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: 93d102de8d685a2ba7418069ea26024963230cf0
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44491704"
---
# <a name="call-records-overview"></a><span data-ttu-id="a565a-103">Visão geral dos registros de chamadas</span><span class="sxs-lookup"><span data-stu-id="a565a-103">Call records overview</span></span>

<span data-ttu-id="a565a-104">Os registros das chamadas fornecem informações de uso e diagnóstico das chamadas e reuniões on-line que ocorrem na sua organização ao usar o Microsoft Teams ou o Skype for Business.</span><span class="sxs-lookup"><span data-stu-id="a565a-104">Call records provide usage and diagnostic information about the calls and online meetings that occur within your organization when using Microsoft Teams or Skype for Business.</span></span> <span data-ttu-id="a565a-105">Os dados de uso e diagnóstico podem ser consumidos para produzir relatórios personalizados para sua empresa para ajudar a monitorar a adoção ou solucionar problemas de qualidade de chamada.</span><span class="sxs-lookup"><span data-stu-id="a565a-105">Usage and diagnostic data can be consumed to produce custom reporting for your business to help monitor adoption or to troubleshoot call quality issues.</span></span>

<span data-ttu-id="a565a-106">As organizações podem assinar alterações em registros de chamadas usando o recurso de [assinaturas de webhook](/graph/api/resources/webhooks?view=graph-rest-1.0) do Microsoft Graph, permitindo que eles criem relatórios quase em tempo real dos dados ou Alertem em determinados cenários, como chamadas de emergência.</span><span class="sxs-lookup"><span data-stu-id="a565a-106">Organizations can subscribe to changes to call records using the Microsoft Graph [webhook subscriptions](/graph/api/resources/webhooks?view=graph-rest-1.0) capability, allowing them to build near-real-time reports from the data or to alert on certain scenarios like emergency calls.</span></span>

> <span data-ttu-id="a565a-107">**Importante:** Use o critério ao conceder a permissão CallRecords. Read. All para aplicativos.</span><span class="sxs-lookup"><span data-stu-id="a565a-107">**Important:** Use discretion when granting the CallRecords.Read.All permission to applications.</span></span> <span data-ttu-id="a565a-108">Os registros de chamadas podem fornecer informações sobre a operação de sua empresa e, portanto, podem ser um alvo de atores mal-intencionados.</span><span class="sxs-lookup"><span data-stu-id="a565a-108">Call records can provide insights into the operation of your business, and therefore can be a target for malicious actors.</span></span> <span data-ttu-id="a565a-109">Conceda essa permissão apenas aos aplicativos que você confia para atenderem aos seus requisitos de proteção de dados.</span><span class="sxs-lookup"><span data-stu-id="a565a-109">Only grant this permission to applications you trust to meet your data protection requirements.</span></span>

## <a name="subscribe-to-call-records"></a><span data-ttu-id="a565a-110">Inscrever-se em registros de chamadas</span><span class="sxs-lookup"><span data-stu-id="a565a-110">Subscribe to call records</span></span>

<span data-ttu-id="a565a-111">As organizações e parceiros geralmente têm suas próprias ferramentas para gerar relatórios sobre chamadas e reuniões online.</span><span class="sxs-lookup"><span data-stu-id="a565a-111">Organizations and partners often have their own tooling for generating reports about calls and online meetings.</span></span> <span data-ttu-id="a565a-112">Usando WebHooks, eles podem receber um feed contínuo de registros de chamadas à medida que são criados.</span><span class="sxs-lookup"><span data-stu-id="a565a-112">Using webhooks, they can receive a continuous feed of call records as they are created.</span></span> <span data-ttu-id="a565a-113">Esse modelo de push permite que as organizações e parceiros criem suas próprias soluções de relatórios em tempo real.</span><span class="sxs-lookup"><span data-stu-id="a565a-113">This push-model enables organizations and partners to build their own real-time reporting solutions.</span></span>

## <a name="look-up-a-call-record-by-its-call-id"></a><span data-ttu-id="a565a-114">Pesquisar um registro de chamadas por ID de chamada</span><span class="sxs-lookup"><span data-stu-id="a565a-114">Look up a call record by its call ID</span></span>

<span data-ttu-id="a565a-115">Os aplicativos podem recuperar um [registro de chamada](/graph/api/resources/callrecords-callrecord?view=graph-rest-1.0) por sua ID.</span><span class="sxs-lookup"><span data-stu-id="a565a-115">Applications can retrieve a [call record](/graph/api/resources/callrecords-callrecord?view=graph-rest-1.0) by its ID.</span></span> <span data-ttu-id="a565a-116">Essa ID pode ser determinada de uma notificação de webhook ou recuperada das ferramentas administrativas.</span><span class="sxs-lookup"><span data-stu-id="a565a-116">This ID can be determined from a webhook notification or retrieved from administrative tools.</span></span>

## <a name="see-also"></a><span data-ttu-id="a565a-117">Confira também</span><span class="sxs-lookup"><span data-stu-id="a565a-117">See also</span></span>

- [<span data-ttu-id="a565a-118">Permissões dos registros de chamadas</span><span class="sxs-lookup"><span data-stu-id="a565a-118">Call records permissions</span></span>](/graph/permissions-reference#call-records-permissions)
