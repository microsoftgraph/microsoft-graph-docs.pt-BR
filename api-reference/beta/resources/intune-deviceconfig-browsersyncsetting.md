---
title: tipo de número browserSyncSetting
description: Allow(Not Configured) or prevent(Block) the syncing of Microsoft Edge Browser settings. Opção para impedir a sincronização entre dispositivos, mas permitir a substituição do usuário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 9ab83353e8192ff62745946cbb40f8297013a959288808b622f0c102e2e3fdcf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54156349"
---
# <a name="browsersyncsetting-enum-type"></a>tipo de número browserSyncSetting

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Allow(Not Configured) or prevent(Block) the syncing of Microsoft Edge Browser settings. Opção para impedir a sincronização entre dispositivos, mas permitir a substituição do usuário.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|notConfigured|0|Padrão – Permitir a sincronização das configurações do navegador entre dispositivos.|
|blockedWithUserOverride|1 |Impedir a sincronização das configurações do navegador entre dispositivos do usuário, permitir a substituição do usuário da configuração.|
|blocked|2|Impedir absolutamente a sincronização das configurações do navegador em dispositivos de usuário.|




